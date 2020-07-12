# DinoGame
This is the replica Of Google Dino Game when browser is accessed offline
# To Understand the Code follow this documentation
Let's Start
# 1. HTML CANVAS
The HTML <canvas> element is used to draw graphics, on the fly, via JavaScript.

The <canvas> element is only a container for graphics. You must use JavaScript to actually draw the graphics.

Canvas has several methods for drawing paths, boxes, circles, text, and adding images.

Here i have used :
<canvas width="700" height="320" style="margin-top: 30px; display: block;margin: auto" id="mycanvas"></canvas>
# 2.FUNCTION TO DRAW ANY OBJECT

            function drawObject(object)
            {
                var currentImageIndex=counter%object.images.length;
                var currentImage=object.images[currentImageIndex];
                try
                {
                    ctx.drawImage(currentImage,object.x-(object.width/2),object.y-(object.height/2),object.width,object.height);
                } catch(er){}
                if(1===object.repeatX)
                {
                    ctx.drawImage(currentImage,object.width + object.x-(object.width/2),object.y-(object.height/2),object.width,object.height);
                }

            }
# 3. Make different objects Like Dragon/Dino , Clouds, Birds, The Moving Land, Hurdles
will continue later...
