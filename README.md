# calculator-javaScript
##javaScript code 
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
