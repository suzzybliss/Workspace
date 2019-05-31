# Workspace
Grid-Rotator Project
<!DOCTYPE html>
<html>
    <head>
        <meta charset="utf-8>"
        
    </head>
    <style>
        body {
            text-align: center
        }
        #btns {
            display: grid;
            grid-template-columns: repeat(3, 100px);
            grid-template-rows: repeat(3, 100px);
            grid-gap: 2px;
            margin: 4px;
        }
    
        button {
            border: 1px solid rgba (10,180,180,1);
            font-size: 18px;
            color: purple;
            text-align: center;
            padding: 0px 0px;
            cursor: pointer;
            transition: 0.2s;        
        }
        
        button:hover{
            background: rgba(20,20,20,0.8);
}
        h1 {
            margin-bottom: 0.8rem;
            font-weight: 500;
            line-height: 1.2;
            margin-top:5px;  
        }
    </style>
    
<body>
    <h1>GRID ROTATOR</h1>
    <label>
        click button 5 to rotate the outer  buttons clockwise and clickon any other button  to rotate the outer buttons anticlockwise
    </label>
    
   <div id="btns" class="container" >
    <button id="btn1" class="button">1</button>
       <button id="btn2" class="button">2</button>
       <button id="btn3" class="button">3</button>
       <button id="btn4" class="button">4</button>
       <button id="btn5" class="button">5</button>
       <button id="btn6" class="button">6</button>
       <button id="btn7" class="button">7</button>
       <button id="btn8" class="button">8</button>
       <button id="btn9" class="button">9</button>
    </div>
    <script>
        btn5.onclick=function () {
        rotate=btn1.innerHTML; btn1.innerHTML=btn4.innerHTML; btn4.innerHTML=btn7.innerHTML; btn7.innerHTML=btn8.innerHTML; btn8.innerHTML=btn9.innerHTML; btn9.innerHTML=btn6.innerHTML; btn6.innerHTML=btn3.innerHTML; btn3.innerHTML=btn2.innerHTML; btn2.innerHTML=rotate;
        }
    </script>
</body>
</html>
