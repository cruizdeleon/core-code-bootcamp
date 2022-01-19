TUESDAY CHALLENGES

function multiply(a, b){
  c=a * b
  return c
}

function uniTotal (string) {
// total up dem unicodes!
  var arr = Array.from(string);
  var sum = 0;
for (var i = 0; i < arr.length; i++)
sum += arr[i].charCodeAt(0); 
console.log(sum);
return sum; 


function getChar(c){
  // ...
  return String.fromCharCode(c)
}

function addBinary(a,b) {
  const sum = a+b;
  return sum.toString(2);

}

function finalGrade (exam, projects) {
  if (exam > 90 && projects >= 10) {
    return 100;
  } else if (exam > 75 && projects >= 5) {
    return 90;
  } else if (exam > 50 && projects >= 2) {
    return 75;
  } else {
    return 0;
  }
  
}
