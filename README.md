# Hacking
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <canvas id="myCanvas" width="640" height="480" style="border:1px solid #000000;">
    </canvas>

    <script type="text/javascript">
        let canvas = document.getElementById("myCanvas");
        let ctx = canvas.getContext("2d");

        // ctx.strokeRect(10, 10, 10, 10);
        // ctx.fillRect(40, 10, 100, 50);
        // ctx.clearRect(50, 10, 20, 40);   

        // ctx.beginPath();
        // ctx.moveTo(20, 20);
        // ctx.lineTo(50, 50);
        // ctx.stroke();

        // ctx.beginPath();
        // ctx.moveTo(100, 100);
        // ctx.lineTo(100, 300);
        // ctx.lineTo(300, 300);
        // ctx.closePath();
        // ctx.stroke();

        // ctx.beginPath();
        // ctx.arc(95, 50, 40, 0, 2*Math.PI, true);
        // ctx.stroke();

        let grd = ctx.createLinearGradient(100,100,100,10);
        grd.addColorStop(0,"red");
        grd.addColorStop(1,"black");

        ctx.fillStyle = grd;
        ctx.fillRect(10,10,150,80);



    
    </script>
    
    var scene = new THREE.Scene();
var camera = new THREE.PerspectiveCamera(75,window.innerWidth / window.innerHeight,0.1,100);
/*
4 parameter:
1.FOV -> field of view yang berarti jarak pandang camera.semakin besar FOV maka semakin jauh jarak pamdang
         kamera dan sebaliknya.
2.Aspect Ratio -> penyesuain terhadap layar yang anda gunakan.
3.near clip -> seberapa dekat yang dapat dilihat oleh camera.
4.far clip -> seberapa jauh yang dapat dilihat oleh kamera.
*/
var renderer = new THREE.WebGLRenderer();

document.body.appendChild(renderer.domElement);
/* menambahkan dom element dari renderer ke index.html */


renderer.setSize( window.innerWidth, window.innerHeight);
/* mengatur size pada layar */
var geometry = new THREE.BoxGeometry(); /* bentuk 3d */
			var material = new THREE.MeshBasicMaterial( { color: 0x00ff00 } );
			var cube = new THREE.Mesh( geometry, material );
			scene.add( cube );

			camera.position.z = 5;

			var animate = function () {
				requestAnimationFrame( animate );

				cube.rotation.x += 0.01;
				cube.rotation.y += 0.01;

				renderer.render( scene, camera );
			};

			animate();
			
			
<?php 
// $_GET
$mahasiswa = [
    [
        "nama" => "You Rio", 
        "nrp" => "0987465390", 
        "email" => "yorio.co@gmail.com",
        "jurusan" => "Teknik Informatika",
        "gambar" => "yorioo.jpg"
    ],
    [
        "nama" => "Yoyo Rio", 
        "nrp" => "098742580", 
        "email" => "yoyorio.co@gmail.com",
        "jurusan" => "Teknik Industri",
        "gambar" => "yourioo.jpg"
    ]
];

?>			
</body>
</html>
