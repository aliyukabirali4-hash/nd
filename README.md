[Uploading muzammil    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Document</title>
        <style>
            body{
                background:aqua;
                display: flex;
                justify-content: center;
                align-items: center;
                height: 100vh;
                color:black;
                margin: 5px;
            
            }
            .calculator{
                background: rgb(0, 0, 20);
                border-radius: 15px;
                padding: 20px;
                text-align: center;
                box-shadow: 2fr;
                width: 360px;
            }
            .display{
                background-color: rgb(243, 237, 237);
                border-radius: 8px;
                font-size: 2.5rem;
                padding: 10px 10px;
                margin-bottom: 25px;
                text-align: right;
                font-weight: bold;
                letter-spacing: 2px;
                color: black;
                user-select: none;
                min-width: 2;
                word-wrap: break-word;
            }
            .buttons{
                display: grid;
                grid-template-columns:repeat(4,1fr);
                gap: 15px;
            }
            button{
            
                border-radius: 10px;
                font-size: 2.5rem;
                padding: 10px; 
                color: azure; 
                background-color:gray;
                font-weight: bold;
                cursor: pointer;
                transition: background 0.3s ease,color 0.3s ease;

            }
            button:hover{
                background: rgb(119, 212, 119);
                color: white;

            }
            .operator{
                background: aqua;
                color: black;
            }
            .operator:hover{
                background: black;
            }
            .equal{
                background: green;

            }
            .equal:hover{
                background: blue;
            }
            .clear{
                background: red;

            }
           .calculator,h1{
            color: aliceblue;
           }
        </style>
    </head>
    <body>
        <ol>
            <li>MUZAMMIL BELLO SAID 0087</li>
            <li>UMMULKHAIRI ALKASIM NABABA 0094</li>
            <li>NAZIRA BELLO ABDULLAHI 0093</li>
            <li>AISHA NAJIB IDRIS 00</li>
            <li>YUSUF ABUBAKAR ABDURRAZAQ 00</li>
            <li>MUHD UMAR MUHD 00</li>
            <li>IBRAHIM MUHD KABIR 00</li>
            <li>ABDULJALEEL NURADDIN 00</li>
            <li>ISAH JIBRIN 00</li>
            <li>ABDULKADIR UMAR MUHD 00</li>
            <li>MAGHILI UMAR IDRIS 00</li>
            <li>SA'IDU MU'AZU MUHAMMAD 0135.</li>
            
        </ol>
        
        <div class="calculator">
            <H1>Calculator group B</H1>
            <div id="display" class="display">0</div>
            <div class="buttons">
              <button class="clear" onclick="clearDisplay()">C</button>
              <button onclick="appendValue('(')">(</button>
              <button onclick="appendValue(')')">)</button>
              <button class="operator" onclick="appendValue('/')">÷</button>
        
              <button onclick="appendValue('7')">7</button>
              <button onclick="appendValue('8')">8</button>
              <button onclick="appendValue('9')">9</button>
              <button class="operator" onclick="appendValue('*')">×</button>
        
              <button onclick="appendValue('4')">4</button>
              <button onclick="appendValue('5')">5</button>
              <button onclick="appendValue('6')">6</button>
              <button class="operator" onclick="appendValue('-')">−</button>
        
              <button onclick="appendValue('1')">1</button>
              <button onclick="appendValue('2')">2</button>
              <button onclick="appendValue('3')">3</button>
              <button class="operator" onclick="appendValue('+')">+</button>
        
              <button onclick="appendValue('00')">00</button>
              <button onclick="appendValue('0')">0</button>
              <button onclick="appendValue('.')">.</button>
              <button class="equal" onclick="calculateResult()">=</button>
            </div>
          </div>
        
          <script>
            const display = document.getElementById('display');
        
            function appendValue(value) {
              if (display.innerText === "0" && value !== ".") {
                display.innerText = value;
              } else {
                display.innerText += value;
              }
            }
        
            function clearDisplay() {
              display.innerText = "0";
            }
        
            function calculateResult() {
              try {
                let expression = display.innerText.replace(/÷/g, '/').replace(/×/g, '*');
                let result = eval(expression);
                display.innerText = result;
              } catch {
                display.innerText = "Kuskure!";
              }
            }
          </script>
        </body>
        </html>.html…]()
