MONDAY CHALLENGES

function likes(names) {
  // TODO
  if (names.length == 0) {
    return "no one likes this";
  } else if (names.length == 1) {
    return names[0] + " likes this";  
  } else if (names.length == 2) {
    return names[0] + " and " + names[1] + " like this";
  } else if (names.length == 3) {
    return names[0] + ", " + names[1] + " and " + names[2] + " like this";
  } else {
    return names[0] + ", " + names[1] + " and " + (names.length - 2) + " others like this";
  }
}

--------------------------BIT COUNTING----------------------------
var countBits = function(n) {
  const base = (n).toString(2).split('');
  const result = base.reduce((sum, num) => sum + Number(num), 0);
  return result; 
};

------------------------MORSE CODE--------------------------------
decodeMorse = function(morseCode){
  function decodeMorseLetter(letter) {
    return MORSE_CODE[letter];
  }
  function decodeMorseWord(word) {
    return word.split(' ').map(decodeMorseLetter).join('');
  }
  return morseCode.trim().split('   ').map(decodeMorseWord).join(' ');
}

"TUESDAY CHALLENGES"

function order(words){
  // ...
   if (words.length == 0){return words}
  let wordsarr = words.split(' ');
  let indarr = words.match(/\d/g);
  let neword = [];
  for (let i=1;i<=indarr.length;i++){
    let ind = indarr.indexOf(i.toString())
    neword.push(wordsarr[ind])
  }
  return neword.join(' ')
}


function duplicateCount(text){
  text = text.toLowerCase().split("")
  const countedletters = text.reduce((allLetters, letter) => {
    if(letter in allLetters) {
    allLetters[letter]++
    } 
    else {
    allLetters[letter] = 1
    }
    return allLetters 
    }, {})
  const filterDup = Object.values(countedletters).filter((duplicate) => duplicate >=2)
  return filterDup.length
}


function pigIt(str){
  str = str.trim().split(/\s{1,}/);
    return str.map(val => {
        if (/^[A-Za-z]+$/.test(val)) {
            return `${val.slice(1)}${val.slice(0, 1)}ay`;
        }
        return val;
    }).join(' ');
}

"WEDNESDAY CHALLENGES"

function validParentheses(parens) {
  var n = 0;
  for (var i = 0; i < parens.length; i++) {
    if (parens[i] == '(') n++;
    if (parens[i] == ')') n--;
    if (n < 0) return false;
  }
  
  return n == 0;
}

function toCamelCase(str){
str = str.split('');
  return str.map(function(el, i){
    if(el == '-' || el == '_'){
      el = str[i+1].toUpperCase();
      str.splice(i+1, 1);
    }
    return el;
  }).join('');
}

var uniqueInOrder=function(iterable){
    var arr = [];
    for (var i=0;i<iterable.length;i++) {

    if (iterable[i] !== iterable[i+1]) {


      arr.push(iterable[i]);
    }
  }
  return arr;
}

"THURSDAY CHALLENGES"

function foldArray(array, runs)
{
  const arrays = [], c = array.slice();
  while (c.length) arrays.push(c.pop() + (c.shift() || 0));
  return runs - 1 ? foldArray(arrays, runs - 1) : arrays;
}

var encryptThis = function(text) {
  if (text==''){
    return '';
      
      }
  else{
    let s= text.split('');
    let x= s.map(element =>{
      let a= element.split('');
      a[0]=element.charCodeAt(0);
      [a[1],a[a.lenght-1]]=[a[a.lenght-1], a[1]];
      return a.join('');});
    return x.join('');
  }
}
******aun me quedó un error*****

const list = names =>
  names.map(x=>x.name)
    .join(', ')
    .replace(/,\s(\w+)$/,' & $1');

