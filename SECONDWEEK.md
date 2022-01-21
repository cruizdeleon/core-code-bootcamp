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

WEDNESDAY CHALLENGES

function dutyFree(normPrice, discount, hol){
  return Math.floor(hol/((normPrice*discount)/100));
}

function twiceAsOld(dadYearsOld, sonYearsOld) {
  // your code here
  let twice = dadYearsOld - sonYearsOld * 2;
return twice < 0 ? twice * (-1) : twice;
}

function validSpacing(s) {
  // write your code here
   return s.replace(/\s{2,}/g, ' ').trim() === s;
}

function fakeBin(x){
  return x.replace(/[1234]/g, '0').replace(/[56789]/g, '1');
}

THURSDAY CHALLENGES

function remove (string) {  
  return string.replace(/!*$/g,'');
}

function shortcut (string) {
  return string.split(/[aeiou]/g).join('')
}

const rps = (p1, p2) => {
  if (p1 === p2) {
    return `Draw!`;
  }
  if (p1 === 'rock' && p2 === 'scissors') {
    return `Player 1 won!`;
  } else if (p1 === 'paper' && p2 === 'rock') {
    return `Player 1 won!`;
  } else if (p1 === 'scissors' && p2 === 'paper') {
    return `Player 1 won!`;
  } else {
    return `Player 2 won!`;
  }
};

function persistence(n):

    count = 0
    temp = 1
    multi = n
    
    while len(str(multi)) > 1:
        for num in str(multi):
            temp *= int(num)
        multi = temp
        temp = 1
        count += 1
    return count
