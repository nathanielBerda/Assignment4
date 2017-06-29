var canvas = document.createElement('canvas');
canvas.width = 500;
canvas.height = 460;
canvas.style.zIndex = 9;
canvas.style.position = "absolute";
canvas.style.border = "2px solid";
canvas.style.marginLeft= "50px";
var body = document.getElementsByTagName("body")[0];
body.appendChild(canvas);



var drawzone = document.createElement('canvas');
drawzone.id= "draw";
drawzone.width = 460;
drawzone.height = 460;
drawzone.style.zIndex = 9;
drawzone.style.position = "absolute";
drawzone.style.border = "2px solid";
drawzone.style.marginLeft= "90px";
drawzone.style.cursor="crosshair";
body.appendChild(drawzone);

var color="black";
var size="3";
//green
var gr = document.createElement('button');
gr.id= "green";
gr.style.width = "20px";
gr.style.height = "20px";
gr.style.zIndex = 9;
gr.style.position = "absolute";
gr.style.border = "2px solid";
gr.style.marginLeft= "50px";
gr.style.backgroundColor="#33cc33"
body.appendChild(gr);
document.getElementById('green').addEventListener("click", green);
function green(){
	color="#33cc33";
	cc.style.backgroundColor=color;
}
//yellow
var ye = document.createElement('button');
ye.id= "yellow";
ye.style.width = "20px";
ye.style.height = "20px";
ye.style.zIndex = 9;
ye.style.position = "absolute";
ye.style.border = "2px solid";
ye.style.marginLeft= "70px";
ye.style.backgroundColor="yellow"
body.appendChild(ye);
document.getElementById('yellow').addEventListener("click", yellow);
function yellow(){
	color="yellow";
	cc.style.backgroundColor=color;
}
//blue
var bl = document.createElement('button');
bl.id= "blue";
bl.style.width = "20px";
bl.style.height = "20px";
bl.style.zIndex = 9;
bl.style.position = "absolute";
bl.style.border = "2px solid";
bl.fillStyle="green";
bl.style.marginLeft= "50px";
bl.style.marginTop= "20px";
bl.style.backgroundColor="blue";
body.appendChild(bl);
document.getElementById('blue').addEventListener("click", blue);
function blue(){
	color="blue";
	cc.style.backgroundColor=color;
}
//orange
var or = document.createElement('button');
or.id= "orange";
or.style.width = "20px";
or.style.height = "20px";
or.style.zIndex = 9;
or.style.position = "absolute";
or.style.border = "2px solid";
or.style.marginLeft= "50px";
or.style.marginTop= "40px";
or.style.backgroundColor="orange";
body.appendChild(or);
document.getElementById('orange').addEventListener("click", orange);
function orange(){
	color="orange";
	cc.style.backgroundColor=color;
}


//red
var re = document.createElement('button');
re.id= "red";
re.style.width = "20px";
re.style.height = "20px";
re.style.zIndex = 9;
re.style.position = "absolute";
re.style.border = "2px solid";
re.style.marginLeft= "70px";
re.style.marginTop= "20px";
re.style.backgroundColor="red"
body.appendChild(re);
document.getElementById('red').addEventListener("click", red);
function red(){
	color="red";
	cc.style.backgroundColor=color;
}


//black
var bla = document.createElement('button');
bla.id= "black";
bla.style.width = "20px";
bla.style.height = "20px";
bla.style.zIndex = 9;
bla.style.position = "absolute";
bla.style.border = "2px solid";
bla.style.marginLeft= "70px";
bla.style.marginTop= "40px";
bla.style.backgroundColor="black"
body.appendChild(bla);
document.getElementById('black').addEventListener("click", black);
function black(){
	color="black";
	cc.style.backgroundColor=color;
	}
	
//purple
var pur = document.createElement('button');
pur.id= "purple";
pur.style.width = "20px";
pur.style.height = "20px";
pur.style.zIndex = 9;
pur.style.position = "absolute";
pur.style.border = "2px solid";
pur.style.marginLeft= "50px";
pur.style.marginTop= "60px";
pur.style.backgroundColor="purple"
body.appendChild(pur);
document.getElementById('purple').addEventListener("click", purple);
function purple(){
	color="purple";
	cc.style.backgroundColor=color;
	}	

//brown
var brow = document.createElement('button');
brow.id= "brown";
brow.style.width = "20px";
brow.style.height = "20px";
brow.style.zIndex = 9;
brow.style.position = "absolute";
brow.style.border = "2px solid";
brow.style.marginLeft= "70px";
brow.style.marginTop= "60px";
brow.style.backgroundColor="brown";
body.appendChild(brow);
document.getElementById('brown').addEventListener("click", brown);
function brown(){
	color="brown";
	cc.style.backgroundColor=color;
}	


//eraser
var era = document.createElement('img');
era.id= "eraser";
era.src="http://img.day.az/2016/12/27/854044.jpg";
era.style.fontSize="10px"
era.style.width = "36px";
era.style.height = "20px";
era.style.zIndex = 9;
era.style.position = "absolute";
era.style.border = "2px solid";
era.style.marginLeft= "50px";
era.style.marginTop= "79px";
era.style.marginBottom="3px"
era.style.paddingLeft="1px";

era.style.cursor ="pointer";
body.appendChild(era);
document.getElementById('eraser').addEventListener("click", eraser);
function eraser(){
	color="white";
}


//sizes
var sizes = document.createElement('P');
sizes.innerHTML="Sizes";
sizes.style.fontSize="15px"
sizes.style.width = "33px";
sizes.style.height = "20px";
sizes.style.zIndex = 9;
sizes.style.position = "absolute";
sizes.style.border = "2px solid";
sizes.style.marginLeft= "51px";
sizes.style.backgroundColor="#c2c2a3";
sizes.style.marginTop= "100px";
sizes.style.paddingLeft="3px"
body.appendChild(sizes);

//small
var sm = document.createElement('button');
sm.id= "small";
sm.innerHTML="Small";
sm.style.fontSize="10px"
sm.style.width = "40px";
sm.style.height = "20px";
sm.style.zIndex = 9;
sm.style.position = "absolute";
sm.style.border = "2px solid";
sm.style.marginLeft= "51px";
sm.style.backgroundColor="White";
sm.style.marginTop= "118px";
sm.style.cursor ="pointer";
body.appendChild(sm);
document.getElementById('small').addEventListener("click", small);
function small(){
	size=3;
}

//medium
var med = document.createElement('button');
med.id= "medium";
med.innerHTML="Medium";
med.style.fontSize="10px"
med.style.width = "40px";
med.style.height = "20px";
med.style.zIndex = 9;
med.style.position = "absolute";
med.style.border = "2px solid";
med.style.backgroundColor="white";
med.style.marginLeft= "51px";
med.style.marginTop= "136px";
med.style.textAlign="center";
med.style.paddingLeft="0px";
med.style.cursor ="pointer";
body.appendChild(med);
document.getElementById('medium').addEventListener("click", medium);
function medium(){
	size=5;
	console.log(size)
}


//big
var bi = document.createElement('button');
bi.id= "big";
bi.innerHTML="Big";
bi.style.fontSize="10px"
bi.style.width = "40px";
bi.style.height = "20px";
bi.style.zIndex = 9;
bi.style.position = "absolute";
bi.style.textAlign="center";
bi.style.border = "2px solid";
bi.style.backgroundColor="white";
bi.style.marginLeft= "51px";
bi.style.marginTop= "154px";
bi.style.cursor ="pointer";
body.appendChild(bi);
document.getElementById('big').addEventListener("click", big);
function big(){
	size=8;
	console.log(size)
}

//clear
var cle = document.createElement('button');
cle.id= "clear";
cle.innerHTML="Clear";
cle.style.fontSize="10px"
cle.style.width = "40px";
cle.style.height = "20px";
cle.style.zIndex = 9;
cle.style.position = "absolute";
cle.style.textAlign="center";
cle.style.border = "2px solid";
cle.style.backgroundColor="white";
cle.style.marginLeft= "51px";
cle.style.marginTop= "185px";
cle.style.cursor ="pointer";
body.appendChild(cle);
document.getElementById('clear').addEventListener("click", clear);
function clear(){
	
	var square=document.getElementById("draw");
	var ctx=square.getContext("2d");
	ctx.clearRect(0, 0, 1000, 1000);
	cc.style.backgroundColor="black";
	color="black";
	}


//colorcheck
var cc= document.createElement('div');
cc.id= "cc";
cc.style.width = "36px";
cc.style.height = "20px";
cc.style.zIndex = 9;
cc.style.position = "absolute";
cc.style.textAlign="center";
cc.style.border = "2px solid";
cc.style.backgroundColor=color;
cc.style.marginLeft= "51px";
cc.style.marginTop= "210px";
body.appendChild(cc);


//rotate
var rotatright = document.createElement('img');
rotatright.src="https://image.freepik.com/free-icon/arrow-pointing-to-right_318-50470.jpg";
rotatright.id= "rotateright";
rotatright.style.fontSize="10px"
rotatright.style.width = "17px";
rotatright.style.height = "18px";
rotatright.style.zIndex = 9;
rotatright.style.position = "absolute";
rotatright.style.textAlign="center";
rotatright.style.border = "2px solid";
rotatright.style.backgroundColor="white";
rotatright.style.marginLeft= "51px";
rotatright.style.marginTop= "234px";
rotatright.style.cursor ="pointer";
body.appendChild(rotatright);

document.getElementById('rotateright').addEventListener("click", rotater);
var rotation = 0;
function rotater(){
var canvas = document.getElementById("draw");
var ctx = canvas.getContext("2d");
rotation = rotation + 90;
canvas.style.transform = "rotate("+rotation +"deg)"

}


var rotatleft = document.createElement('img');
rotatleft.src="https://image.freepik.com/free-icon/curve-arrow-pointing-to-the-left_318-40238.jpg";
rotatleft.id= "rotateleft";
rotatleft.style.fontSize="10px"
rotatleft.style.width = "17px";
rotatleft.style.height = "18px";
rotatleft.style.zIndex = 9;
rotatleft.style.position = "absolute";
rotatleft.style.textAlign="center";
rotatleft.style.border = "2px solid";
rotatleft.style.backgroundColor="white";
rotatleft.style.marginLeft= "71px";
rotatleft.style.marginTop= "234px";
rotatleft.style.cursor ="pointer";
body.appendChild(rotatleft);

document.getElementById('rotateleft').addEventListener("click", rotatel);
function rotatel(){
var canvas = document.getElementById("draw");
var ctx = canvas.getContext("2d");
rotation = rotation +270;
canvas.style.transform = "rotate("+rotation +"deg)";

}




draw.addEventListener("mousemove", myFunction);

function myFunction(click){
	if (click.buttons ==! 1) return;
var x = event.clientX;
console.log(x);
var y = event.clientY;
console.log(y);
var square=document.getElementById("draw");
var ctx=square.getContext("2d");
	ctx.beginPath();
	ctx.lineWidth = size;
	ctx.fillStyle=color;
	var r=rotation/90;
	console.log(r);
if(r%4==0){
		ctx.fillRect(x-100,y-10,size,size);
}
else if(r%4==1){
		ctx.fillRect(y-10,557-x,size,size);	
	
}
else if(r%4==2){
	ctx.fillRect(-x+560,-y+470,size,size);
	
}
else if(r%4==3){
	ctx.fillRect(470-y,x-100,size,size);
		console.log("ok");
}
	

}