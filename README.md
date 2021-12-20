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
