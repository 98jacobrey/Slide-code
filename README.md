# Slide-code
Simple button and slide code

<style>
.tabs{
    font-size: 20px;
}
.info{
    display: none;
}
.title{
  color: white;
  grid-area: 1/1/4/5;
  font-size: 30px;
}
.nav{
  display: grid;
  min-height: 80px;
  width: 98.8%;
  margin: auto;
  background:black;
  grid-template-columns: 1fr auto;
  grid-gap: 3px;
  grid-template-areas:
  "title . . . .";
}
</style>

<html>
<nav class="nav">
<h2 class="title">Jacob Autrey</h2>
<button class="tabs" onClick="showInfo(1)">About me</button>
<button class="tabs" onClick="showInfo(2)">Projects</button>
<button class="tabs" onClick="showInfo(3)">References</button>
<button class="tabs" onClick="showInfo(4)">Contact Me</button>
</nav>

<div class= "content">
<div class = "info">blachsdjpiashdfdfjhgsdf</div>
<div class = "info">oshdofhsofhosdhf</div>
<div class = "info">foiusfdyihdfuffds</div>
<div class = "info">jmsdijadojiaodjh</div>
</div>
</html>


<script>
  var infoIndex = 1;
  showInfo(infoIndex);

  function showInfo(n){
    var i;
    var info = document.getElementsByClassName("info")
    infoIndex = n
    for(i = 0; i < info.length; i++){
      info[i].style.display = "none"
    }
    info[infoIndex-1].style.display = "block"
  }
</script>
