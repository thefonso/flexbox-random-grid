### Random grid example

Just a basic example to demonstrate what can be done quickly with flexbox. Could be used as a starting point to a more advanced layout.

Uses the nth-child() selector to explicitly set sizes on some of the flex items, but this can be changed to classes if required

```html
<!doctype html>
<title>Example</title>
<style>
 * {
   box-sizing: border-box;
  }
.container { 
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  height: 100vh;
  flex-wrap: wrap;
  } 
.container > div {
  font-size: 5vw;
  padding: .5em;
  color: white;
  margin: 10px;
  border-radius: 3px;
  background: yellowgreen;
  border: 5px solid black;
}
.container > div:nth-child(odd) {
  width: 10%;
  }
.container > div:nth-child(even) {
  width: 20%;
  }
.container > div:nth-child(2),
.container > div:nth-child(4),
.container > div:nth-child(9) {
  width: 60%;
  }  
body {
  margin: 0;
}
</style>
<div class="container">
  <div></div>
  <div></div>
  <div></div>
  <div></div>
  <div></div>
  <div></div>
  <div></div>
  <div></div>
  <div></div>
  <div></div>
  <div></div>
  <div></div>
  <div></div>
  <div></div>
</div>
```
