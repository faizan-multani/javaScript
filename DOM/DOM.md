# DOM : Document Object Model
- when a page is loaded , the browser creates a document object model of the page.

## Advantages : 
- readability.
- modular.
- helps browser caching(loading time will be faster).

## window :
- it is an object , represents an open window in browser.
- browser creates it automatically.
- it is global object with properties and methods.

### Note :
```
<body>
<h1>hello world</h1>
<p>lorem para</p>

<script></script>
</body>
```
- make sure always wirte ' script ' tag before closing ' body ' tag.
- becoz it improves the page loading speed.
- avoid blocking rendering.
- Access to dom elelment.

## DOM Manipulation :
- we can manipulate dom element by using dom perperties.

## 1. Selecting Elements :
- getElementById() , getElementsByClassName() , getElementsByTagName(), querySelector() , querySelectorAll().

### getElementById() :
```
const header = document.getElementById('myHeader');
```

## 2. Modifying Content :
### innerHTML :
- Allows you to get or set the HTML content inside an element.
```
const content = document.getElementById('myContent').innerHTML;
document.getElementById('myContent').innerHTML = "<p>New content</p>";
```

### textContent :
- Similar to innerHTML, but only deals with text, not HTML markup.
```
const text = document.getElementById('myText').textContent;
document.getElementById('myText').textContent = "Updated text!";
```

## 4. Adding and Removing Elements :
### createElement() :
- Creates a new HTML element.
```
const newDiv = document.createElement('div');
newDiv.innerHTML = "<p>This is a new div!</p>";
document.body.appendChild(newDiv);

// appendChild(): Adds a new element as a child of an existing element.
```

### removeChild() :
- Removes a child element from a parent.
```
const parent = document.getElementById('parent');
const child = document.getElementById('child');
parent.removeChild(child);
```

