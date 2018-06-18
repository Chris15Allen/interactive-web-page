# interactive-web-page
<!DOCTYPE html>
<html>
    <head>
        <title>An interactive web page</title>
        <style>
            #color_box {width: 200px; height: 200px;}
            .gray {background: gray;}
            .blue {background: rgb(67, 111, 255);}
            .pink {background: pink;}
        </style>
    </head>
    <body>
        <h1>An interactive web page</h1>

        <h2>1. Color changer</h2>
        <button id="gray_button">Gray</button>
        <button id="blue_button">Blue</button>
        <button id="pink_button">Pink</button>
        <div id="color_box" class="gray"></div>        
        <script>
            const gray_button = document.getElementById("gray_button");
            const blue_button = document.getElementById("blue_button");
            const pink_buttom = document.getElementById("pink_button");
            const color_box = document.getElementById("color_box");
            gray_button.onclick = function() {
                color_box.className = "gray";
            };
            blue_button.onclick = function () {
                color_box.className = "blue";
            }
            pink_buttom.onclick = function() {
                color_box.className = "pink";
            }

            /* TODO 1
             *
             * Add a third button (and the associated event handler)
             * to support an additional color: pink
             */
        </script>

        <hr>

        <h2>2. Counter</h2>
        <button id="counter_button">This fabulous button</button>
        has been clicked <span id="countspan">0</span> times.
        <script>
            var count=0;
            const counter_button = document.getElementById("counter_button");
            const countspan = document.getElementById("countspan");
            counter_button.onclick = function() { 
                count++
                countspan.textContent =  count 
                
              
                /* TODO 2
                 *
                 * Fill in this function so that it increments
                 * (adds one to) the variable named count,
                 * then updates the text content of "countspan"
                 * to show the current value of "count".
                 */
            }
        </script>

        <hr>

        <h2>3. Even or Odd?</h2>
        <button id="even_or_odd_button">Is the count even or odd?</button>
        <script>
            const even_or_odd_button = document.getElementById("even_or_odd_button");
            even_or_odd_button.onclick = function(an) {
                
                
                if(count % 2 === 0 ){
                alert('count is even');}
                    else 
                    alert('count is odd')};

              
                /* TODO 3
                 *
                 * Fill in this function so that it shows an
                 * alert dialog stating whether the count
                 * (from part 2, above) is even or odd.
                 */
            
        </script>
    </body>
</html>
