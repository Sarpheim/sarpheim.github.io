<html lang="tr">
  <head>
    <meta charset="UTF-8">
      <link rel="icon" href="http://www.sarpheimbot.tk/images/sarp-karakaya/Sarpheim_Logo.png">
      <title>Sarpheim Reddit r/place</title>
      <style>
        body {
          background-color: #AAAAAA;
        }
        .container {
          position: relative;
        }
        .container > canvas {
          position: absolute;
          top: 0;
          left: 0;
        }
        h1 {
          font-size: 1.5rem;
          color: #000000;
          font: 700 1.25rem/2.125rem "Montserrat", sans-serif;
          margin-top: 0px;
          margin-bottom: 0px;
        }
        h2 {
          font-size: 1.25rem;
          color: #000000;
          font: 700 1.125rem/1.625rem "Montserrat", sans-serif;
          margin-top: 0px;
          margin-bottom: 0px;
        }
      </style>
    </head>
    <body>
      <h1>Colors</h1>
      <h2>- Black</h2>
      <h2>- Light Blue</h2>
      <div id="container" class="container">
        <canvas id="canvas_background" width="25" height="25"></canvas>
        <canvas id="canvas_foreground" width="25" height="25"></canvas>
      </div>
      
      <script>
        const X_PIXELS = 50
        const Y_PIXELS = 50
        const X_OFFSET = 25
        const Y_OFFSET = 25
        const X_IN_PLACE = 0
        const Y_IN_PLACE = 0

        function getMousePos(canvas, evt) {
          const rect = canvas.getBoundingClientRect()
          return {
            x: (evt.clientX - rect.left) / (rect.right - rect.left) * canvas.width,
            y: (evt.clientY - rect.top) / (rect.bottom - rect.top) * canvas.height
          }
        }
        function drawGrid(x_0, y_0, x_max, y_max, ctx) {
          for (let x = x_0; x <= x_max; x += X_PIXELS) {
            ctx.moveTo(x, y_0)
            ctx.lineTo(x, y_max)
            for (let y = y_0; y <= y_max; y += Y_PIXELS) {
              ctx.moveTo(x_0, y)
              ctx.lineTo(x_max, y)
            }
          }
          ctx.strokeStyle = "#535353"
          ctx.stroke()
        }
        
        const background = document.getElementById("canvas_background")
        const bg = background.getContext("2d")
        
        const foreground = document.getElementById("canvas_foreground")
        const fg = foreground.getContext("2d")

        const img = new Image()
        img.onload = function() {
          w = img.width * X_PIXELS
          h = img.height * Y_PIXELS

          bg.canvas.width  = w + X_OFFSET
          bg.canvas.height = h + 2 * Y_OFFSET

          fg.canvas.width = bg.canvas.width
          fg.canvas.height = bg.canvas.height
          bg.imageSmoothingEnabled = false
          bg.drawImage(img, 0, 0, img.width, img.height, 0, Y_OFFSET, w, h)
          drawGrid(0, Y_OFFSET, w, h + Y_OFFSET, bg)
      }
      img.src = "data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABkAAAAZCAYAAADE6YVjAAAAAXNSR0IArs4c6QAAAK5JREFUSEvtlUkOwCAIReUSvf/5vISNphhqmBzY2a2FJ5+PQMqlpOAPGuSBOEwu6UL88k7JlQ1/SH11QywA1sWBRAgmrUEjYEzkOOfdJUEUSXqTmEv4IdYs0YtRW0zLpYGOQYwGt+MluWqg5i5MulXJOHYckLpwuRJuviksDEJl3IJwjcSqjlUiuYmb8unGW46iPXIMqb60rIfRAnyXvZsxaDP60/7/7K/wagJn3AuwRMDCPDsaRwAAAABJRU5ErkJggg=="
        function drawText(text, x, y){
          fg.font = "30px Sans-serif"
          fg.strokeStyle = "black"
          fg.lineWidth = 8
          fg.strokeText(text, x, y)
          fg.fillStyle = "white"
          fg.fillText(text, x, y)
      }

      foreground.addEventListener("mousemove", (event) => {
        let p = getMousePos(foreground, event)
        let x = Math.floor((p.x) / X_PIXELS)
        let y = Math.floor((p.y - Y_OFFSET) / Y_PIXELS) 
        
        fg.clearRect(0, 0, fg.canvas.width, fg.canvas.height)
        
        if (y < 0 || x < 0 || y > 24 || x > 24) {
          return;
        }
        drawText(`(${(x + X_IN_PLACE)},${(y + Y_IN_PLACE)})`, p.x - 40, p.y - 30)
        
        fg.lineWidth = 5
        let circle_x = x * X_PIXELS + X_PIXELS / 2
        let circle_y = y * Y_PIXELS + Y_OFFSET + Y_PIXELS / 2
        fg.beginPath()
        fg.strokeStyle = "#00EAFF"
        fg.arc(circle_x, circle_y, X_PIXELS - 6, 0, 2 * Math.PI, false)
        fg.stroke()
        
        fg.beginPath()
        fg.strokeStyle = "#FFFFFF"
        fg.arc(circle_x, circle_y, X_PIXELS - 4, 0, 2 * Math.PI, false)
        fg.stroke()
        
        fg.beginPath()
        fg.strokeStyle = "#000000"
        fg.arc(circle_x, circle_y, X_PIXELS, 0, 2 * Math.PI, false)
        fg.stroke()
      })

      foreground.addEventListener("click", (event) => {
        let p = getMousePos(foreground, event)
        let x = Math.floor((p.x) / X_PIXELS) + X_IN_PLACE
        let y = Math.floor((p.y) / Y_PIXELS) + Y_IN_PLACE

        if (y < Y_IN_PLACE || x < X_IN_PLACE) {
          return;
        }
        
        window.open(`https://www.reddit.com/r/place/?cx=${x}&cy=${y}&px=20`, "_blank").focus()
      })
    </script>
  </body>
</html>
