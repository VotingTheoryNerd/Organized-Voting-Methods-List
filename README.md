# Organized-Voting-Methods-List
A comprehensive collapsible list of voting methods in an organized fashion.
<!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1">
<style>
.collapsible {
  background-color: #777;
  color: white;
  cursor: pointer;
  padding: 18px;
  width: 100%;
  border: none;
  text-align: left;
  outline: none;
  font-size: 15px;
}

.active, .collapsible:hover {
  background-color: #555;
}

.content {
  padding: 0 18px;
  display: none;
  overflow: hidden;
  background-color: #f1f1f1;
}
</style>
</head>
<body>

<h2>Voting Methods</h2>

<p>Single-Winner Methods</p>
<button class="collapsible">Single-Choice</button>
<div class="content">
	<button class="collapsible">Rounds</button>
	<div class="content">
    	<button class="collapsible">Top-Two</button>
		<div class="content">
        	<button class="collapsible">Open Section 2</button>
			<div class="content">


<script>
var coll = document.getElementsByClassName("collapsible");
var i;

for (i = 0; i < coll.length; i++) {
  coll[i].addEventListener("click", function() {
    this.classList.toggle("active");
    var content = this.nextElementSibling;
    if (content.style.display === "block") {
      content.style.display = "none";
    } else {
      content.style.display = "block";
    }
  });
}
</script>

</body>
</html>
