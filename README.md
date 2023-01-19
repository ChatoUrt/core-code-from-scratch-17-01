# core-code-from-scratch-17-01

## ---Even/Odd---

* [Test](https://www.codewars.com/kata/53da3dbb4a5168369a0000fe/train/javascript)

Solution1 / /

``` javascript
funtion evenOrOdd(number) {
  const result = number % 2;
  if (Math.abs(result) == 1) {
    return "Even";
  } 
  retunr "Odd";
}

```

Solution2 / /

``` javascript
funtion evenOrOdd(number) {
  return number % 2 ? "Odd" : "Even";
}

```

---
## ---A wolf in sheep's clothing---
* [Test](https://www.codewars.com/kata/5c8bfa44b9d1192e1ebd3d15/train/javascript)

Solution1 / /
 ``` javascript 
function warnTheSheep(queue) {
  const wolf = queue.indexOf('wolf');
  if (wolf === queue.length - 1)
    return "Pls go away and stop eating my sheep";
  const sheep = queue.length - (wolf + 1);
    return `Oi! Sheep number ${sheep}! You are about to be eaten by a wolf!`;
}
 ```
 
 Solution2 / /
 
 ``` javascript
function warnTheSheep(queue) {
  const position = queue.reverse().indexOf('wolf');
  return position === 0 ? "Pls go aways and stop eating my sheeps" : `Oi, Sheep number ${position}! You are about to be eaten by a wolf`;
}
 ```

---
## ---Morse Code---

* [Test](https://www.codewars.com/kata/54b724efac3d5402db00065e/train/javascript)

Resources / /
* [Trim()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/trim)
* [Split()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/split)
* [Join](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/join)
* [Morse Code](https://en.wikipedia.org/wiki/Morse_code)

Solution / /

``` javascript
decodeMorse = function (morseCode) {
  let sentence = [];
  let word = morseCode.trim().split('   ');
  let letters = [];
  for (let i = 0; i < word.length; i++) {
    letters = word[i].split(' ');
    for (let j = 0; j < letters.length; j++) {
     letters[j] = MORSE_CODE[letters[j]];
    }
    sentence.push(letters.join(''));
  }
  return sentence.join(' ').trim();
};
```

---
## ---Knowledge Base---

1.
1.1. [Odd Nums](https://byjus.com/maths/odd-numbers/)<br>
1.2. [Even Nums](https://byjus.com/maths/even-numbers/)<br>
1.3. [MDN Reimainder (%)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Remainder)<br>

2. [Array.indexOf()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/indexOf)<br>

