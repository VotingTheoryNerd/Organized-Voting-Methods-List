var ContentOpacity = '1';
var TimeToSlide = 250.0;

var openAccordion = '';

function runAccordion(index)
{
  var nID = "Accordion" + index + "Content";
  if(openAccordion == nID)
    nID = '';
    
  setTimeout("animate(" + new Date().getTime() + "," + TimeToSlide + ",'" + openAccordion + "','" + nID + "')", 33);
  
  openAccordion = nID;
}

function animate(lastTick, timeLeft, closingId, openingId)
{  
  var curTick = new Date().getTime();
  var elapsedTicks = curTick - lastTick;
  
  var opening = (openingId == '') ? null : document.getElementById(openingId);
  var closing = (closingId == '') ? null : document.getElementById(closingId);
 
  if(timeLeft <= elapsedTicks)
  {
    if(opening != null)
      opening.style.opacity = ContentOpacity;
	  
    if(closing != null)
    {
      closing.style.display = 'none';
	  closing.style.opacity = '0';
    }
    return;
  }
 
  timeLeft -= elapsedTicks;
  var newClosedOpacity = ((timeLeft/TimeToSlide) * ContentOpacity);

  if(opening != null)
  {
    opening.style.display = 'block';
	opening.style.opacity = (ContentOpacity - newClosedOpacity);
  }
  
  if(closing != null)
    closing.style.opacity = newClosedOpacity;

  setTimeout("animate(" + curTick + "," + timeLeft +",'" + closingId + "','" + openingId + "')", 33);
}
