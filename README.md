# calculator-javaScript
## javaScript code 
```javaScript
function Solve(val) {
    var v = document.getElementById('res');
    v.value += val;

 }
const Result=()=> {
    let num1 = document.getElementById('res').value;
    let num2 = eval(num1);
    document.getElementById('res').value = num2;
 }
 const Clear=() =>{
    let inp = document.getElementById('res');
    inp.value = '';
 }
 const Back=()=> {
    let  ev = document.getElementById('res');
    ev.value = ev.value.slice(0,-1);
 }  
```
## html code 
```html
<!DOCTYPE html>
<html lang="en">
<head>
   <link rel="stylesheet" href="style.css">
   <title>Calulator</title>
</head>
<body>
   <div class="main">
      <input type="text" id = 'res'>
      <div class="btn">
         <input type="button" value = 'C' onclick = "Clear()" class="btn-operator">
         <input type="button" value = '%' onclick = "Solve('%')" class="btn-operator">
         <input type="button" value = '←' onclick ="Back('←')" class="btn-operator">
         <input type="button" value = '/' onclick = "Solve('/')" class="btn-operator">
         <br>
         <input type="button" value = '7' onclick = "Solve('7')" class="btn-number">
         <input type="button" value = '8' onclick = "Solve('8')"  class="btn-number">
         <input type="button" value = '9' onclick = "Solve('9')"  class="btn-number">
         <input type="button" value = 'x' onclick = "Solve('*')" class="btn-operator">
         <br>
         <input type="button" value = '4' onclick = "Solve('4')" class="btn-number">
         <input type="button" value = '5' onclick = "Solve('5')" class="btn-number">
         <input type="button" value = '6' onclick = "Solve('6')" class="btn-number">
         <input type="button" value = '-' onclick = "Solve('-')" class="btn-operator">
         <br>
         <input type="button" value = '1' onclick = "Solve('1')" class="btn-number">
         <input type="button" value = '2' onclick = "Solve('2')" class="btn-number">
         <input type="button" value = '3' onclick = "Solve('3')" class="btn-number">
         <input type="button" value = '+' onclick = "Solve('+')" class="btn-operator">
         <br>
         <input type="button" value = '00'onclick = "Solve('00')" class="btn-number">
         <input type="button" value = '0' onclick = "Solve('0')" class="btn-number">
         <input type="button" value = '.' onclick = "Solve('.')" class="btn-number">
         <input type="button" value = '=' onclick = "Result()" class="btn-operator">
      </div>
   </div>
   <script src = 'Calc.js' ></script>
</body>
</html>
```

## css 
```css
*{
    padding: 0;
    margin: 0;
    font-family: 'poppins', sans-serif;
 }
 body{
    background-color: #495250;
    display: grid;
    height: 100vh;
    place-items: center;
 }
 .main{
    width: 400px;
    height: 450px;
    background-color: white;
    position: absolute;
    border: 5px solid black;
    border-radius: 6px; 
 }
 .main input[type='text'] {
    width: 88%;
    position: relative;
    height: 80px;
    top: 5px;
    text-align: right;
    padding: 3px 6px;
    outline: none;
    font-size: 40px;
    border: 5px solid black;
    display: flex;
    margin: auto;
    border-radius: 6px;
    color: black;
 }
 .btn input[type='button']{
    width:90px;
    padding: 2px;
    margin: 2px 0px;
    position: relative;
    left: 13px;
    top: 20px;
    height: 60px;
    cursor: pointer;
    font-size: 18px;
    transition: 0.5s;
    border-radius: 6px;
    color: white;
 }
 .btn-number{
    background-color: #495250;
 }
 .btn input[type='button']:hover{
    background-color: black;
    color: white;
 }
 .btn-operator {
    background-color: #128094;
    color: #ffffff;
}
```
