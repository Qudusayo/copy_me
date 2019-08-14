# copy_me
Copy toclipboard

The Copy Me is a simple JS code which allows you to add a **copy** event to your code for easy copy in your website or webapp. 

## Installation
``` 
npm install copyme --save
 ```
+ After installation, add `<script src="node_modules/copyme/copyMe.min.js"></script>` to your code 


## How It Works
- Add the `<script src="node_modules/copyme/copyMe.min.js"></script>` to your HTML file

- Create any _element_ you want to copy from giving it an _**id**_.

    - E.g ` <div id='copyMe'>The text here will be copied</div> `

- Create an **_eventListener_** on an element that alters the copy Event with a specific _**id**_

    - E.g ` <button id='copy'>Copy</button> `
<br/>
<br/>

### Add This to your JS file
In your js file, add an eventListener listening your element (e.g the button) either (click, mouseover, contextmenu....) . Then call the `copyToClipboard()` function taking the *id* of the item(`#copyMe`) you want to copy as the **parameter**.<br/><br/>
**Sample  Code** <br/>
```html
<body>
    <div id='copyMe'>The text here will be copied</div>
    <button id='copy'>Copy</button>

    <script src="node_modules/copyme/copyMe.min.js"></script>
</body>
```
```js
document.querySelector('#copy').addEventListener('click', function(){
   copyToClipboard(document.querySelector('copyMe'))
});
```
