# JavaScriptHomeWork
 Belhard
 
 
## Naming

  - Use Random in object .

    > 6_1. Заполните новый массив случайными 10-ю числами в диапазоне от 1 до 100.


    ```js
    
    <script>

        let max = 100;
        let random = []; 

        for (let i = 0 ; i < 10 ; i ++ ) {
			let temp = Math.floor (Math.random () * max); 

			if (random.indexOf (temp) == -1) {
				random.push (temp); 
				} 
			else i++; 

            p1.innerHTML= random ;
        };

    </script>
    
    ```
    
    - Use Random in object .
    
       > 6_2. Напишите скрипт, который с помощью функции создает столько блоков 250 х 250 пикселей, сколько введено в prompt и раскрашивает каждый блок рандомным цветом, размещает в центр блоков картинки 100 х 100 пикс.


    ```js
    <!--  <style>
        div.box {width:200px; height: 200px; float:left; margin: 0 50px 50px 0}
 </style>
 <body>
    <button>Push me...</button> <br><br>
    <div id="container"></div>
 </body> -->
    
    <script>

        function onClick() {
            const div = document.createElement("div");
             div.classList.add("box");
             div.style = "background-color: " +'#' + (Math.random().toString(16) + '000000').substring(2,8).toUpperCase();
              document.getElementById("container").appendChild(div);
 
        };
        document.querySelector("button").addEventListener("click", onClick);
        for(let i = 5; i > 0; i--) onClick();

    </script>
    
    ```
