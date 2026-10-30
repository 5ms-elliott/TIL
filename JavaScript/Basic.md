## オブジェクトの値を取得する 
### ２種類の方法 
①ドット記法 
```
const obj = { 
  firstName: "John", 
  age: 25, 
  country: "America", 
}; 

console.log(obj.firstName); // John 
```
 
②ブラケット記法 
```
const obj = { 
  firstName: "John", 
  age: 25, 
  country: "America", 
};

console.log(obj['firstName']); // John 
 
const hoge = 'age'; 
console.log(obj[hoge]); // 25
```
