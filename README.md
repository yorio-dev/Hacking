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
</body>
</html>
