<html>
<head>
<title>PPO Daily Attendance List</title>
<meta http-equiv = "refresh" content = "30; url = external.html" />
</head>
<body>

<div id="datacontainer" style="position:absolute;left:1px;top:10px;width:100%" onMouseover="scrollspeed=cache" onMouseout="scrollspeed=cache">

<!-- ADD YOUR SCROLLER CONTENT INSIDE HERE -->
<style>
#myIframe {
  width: 1920px;
  height: 2000px;
  display: block;
  margin: 0 auto;
  border: 0px;
  text-align:center;
}

#myIframe {
  zoom: 0.75;
  -moz-transform: scale(0.75);
  -moz-transform-origin: 0 0;
  -o-transform: scale(0.75);
  -o-transform-origin: 0 0;
  -webkit-transform: scale(0.75);
  -webkit-transform-origin: 0 0;
}

@media screen and (-webkit-min-device-pixel-ratio:0) {
  #myIframe {
    zoom: 1;
  }
}
</style>

<iframe id="myIframe" src="https://docs.google.com/spreadsheets/d/e/2PACX-1vTDoEWkrDC7iVZG3I1SlxPEhfnN8E-rYDSeoVJu5k4R5EVomlJnqNDyHa6PsFqlVte2JP3-UW6GuRuq/pubhtml?gid=1731893939&amp;" height="2500px" align="middle"></iframe>

<!-- END SCROLLER CONTENT -->

</div>
<img src="file:///C:/Users/gumel/Pictures/Pertamina.png"/>
<script type="text/javascript">

/***********************************************
* IFRAME Scroller script- (c) Dynamic Drive DHTML code library (www.dynamicdrive.com)
* Please keep this notice intact
* Visit Dynamic Drive at http://www.dynamicdrive.com/ for full source code
***********************************************/

//Specify speed of scroll. Larger=faster (ie: 5)
var scrollspeed=cache=1

//Specify intial delay before scroller starts scrolling (in miliseconds):
var initialdelay=5000
var node=0


function initializeScroller(){
dataobj=document.all? document.all.datacontainer : document.getElementById("datacontainer")
dataobj.style.top="5px"
setTimeout("getdataheight()", initialdelay)
}

function getdataheight(){
thelength=dataobj.offsetHeight
if (thelength==0)
setTimeout("getdataheight()",30)
else
scrollDiv()
}

function scrollDiv(){
dataobj.style.top=parseInt(dataobj.style.top)-scrollspeed+"px"
if (parseInt(dataobj.style.top)<thelength*(-1))
dataobj.style.top="5px"
setTimeout("scrollDiv()",30)
}

if (window.addEventListener)
window.addEventListener("load", initializeScroller, false)
else if (window.attachEvent)
window.attachEvent("onload", initializeScroller)
else
window.onload=initializeScroller

</script>

</body>
</html>