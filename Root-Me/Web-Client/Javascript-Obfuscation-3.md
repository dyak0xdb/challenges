# Root-Me – Javascript Obfuscation 3

🔗 Challenge  
https://www.root-me.org/en/Challenges/Web-Client/Javascript-Obfuscation-3

---

## Decode Hex → ASCII

```js
function decodeOctal(str) {
  return str.replace(/\\([0-7]{1,3})/g, (_, oct) =>
    String.fromCharCode(parseInt(oct, 8))
  );
}

// Example
decodeOctal("\x35\x35\x2c\x35\x36\x2c\x35\x34");
````

---

## Convert Decimal ASCII to Plain Text

```js
let enc = "55,56,54,79,115,69,114,116,107,49,50";

const plain = enc
  .split(',')
  .map(n => String.fromCharCode(Number(n)))
  .join('');

console.log(plain); // 786OsErtk12
```
بگو 🔥
```
