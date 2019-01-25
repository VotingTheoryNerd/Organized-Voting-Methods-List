<script type="text/javascript" src="//ajax.googleapis.com/ajax/libs/jquery/1/jquery.min.js"></script>

<script>
$(document).ready(function(){
$('.markdown-block .sqs-block-content h2').css('cursor','pointer');
$(".markdown-block .sqs-block-content h2").nextUntil("h2").slideToggle();
$(".markdown-block .sqs-block-content h2").click(function() {$(this).nextUntil("h2").slideToggle();});
});
</script>


  .sqs-block-markdown h2 {
  border: solid 1px #000;
  padding: 12px 14px;

}



