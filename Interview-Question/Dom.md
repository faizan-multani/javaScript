## Question 1 :  What is the DOM?
- The DOM (Document Object Model) is an API (Application Programming Interface) that represents the structure of an HTML or XML document as a tree of objects. Each object represents a part of the document, such as an element, attribute, or text node. JavaScript can be used to manipulate and interact with the DOM to update content, structure, and style dynamically.

## Question 2 : Explain the difference between document.getElementById() and document.querySelector()?
- document.getElementById(id): Selects an element by its ID. It returns the first element with the specified ID, or null if no such element is found.
- document.querySelector(selector): Selects the first element that matches a CSS selector (e.g., #id, .class, div). It can be used to select elements by tag name, class, or id, and even more complex selectors.
- Key difference: getElementById() can only select by ID, while querySelector() can select by any valid CSS selector.

## Question 3 : What is the difference between getElementsByClassName() and querySelectorAll()?
- getElementsByClassName(className): Returns a live HTMLCollection of elements with the given class name. This means that if the DOM changes (elements are added or removed), the HTMLCollection will automatically update.
- querySelectorAll(selector): Returns a static NodeList of all elements that match the CSS selector. Unlike getElementsByClassName(), it doesn't update when the DOM changes.
- Key difference: getElementsByClassName() is live, whereas querySelectorAll() is static.

## Question 4 :  What is event delegation in the DOM?
- Event delegation is a technique in which an event listener is added to a parent element instead of individual child elements. This allows you to handle events on child elements without attaching listeners to each one individually. The event listener takes advantage of event bubbling, where the event propagates from the target element to the parent elements, allowing you to catch and handle the event on the parent.

- Example :
```

````

## Question 5 : What are the different types of nodes in the DOM?
- Element Nodes: Represent HTML elements (like div, p, etc.).
- Text Nodes: Represent text content inside an element.
- Attribute Nodes: Represent attributes of an element (like class, id, etc.).
- Comment Nodes: Represent comments inside the document.

## Question 6 : How do you select elements using the DOM?
- Elements can be selected using various DOM methods :
- document.getElementById(): Selects an element by its id.

- document.getElementsByClassName(): Selects elements by their class name.

- document.getElementsByTagName(): Selects elements by their tag name.

- document.querySelector(): Selects the first matching element based on a CSS selector.

- document.querySelectorAll(): Selects all matching elements based on a CSS selector.

## Question 7 : What is event bubbling and event capturing in the DOM?
- Event Bubbling: When an event is triggered on an element, it bubbles up from the target element to its ancestors in the DOM tree.

- Event Capturing: The event starts from the root of the DOM and goes down to the target element. By default, events bubble, but you can use the third argument of addEventListener() to enable capturing.

## Question 8 : How can you modify an element’s content in the DOM?
- innerHTML: Sets or gets the HTML content inside an element.
```
// Get the element by ID
const element = document.getElementById('myElement');

// Modify the HTML content
element.innerHTML = '<strong>New Content with HTML</strong>';
```

- textContent: Sets or gets the plain text content inside an element.
```
// Get the element by ID
const element = document.getElementById('myElement');

// Modify the text content
element.textContent = 'New Text Content';
```
- value: Used to get or set the value of input elements like ' input ' or  ' textarea '.

## Summary of Methods :
- textContent: Modify plain text content.

- innerHTML: Modify HTML content inside the element (including tags).

- innerText: Modify text content, taking into account CSS styles.

- value: Modify the value of form elements (input, textarea, etc.).

- setAttribute: Modify attributes like src, href, etc.

- appendChild() / prepend(): Add elements to the DOM.

- replaceWith() / replaceChild(): Replace elements in the DOM.

- style: Modify the inline CSS styles of an element.

## Question 9 : What are DOM manipulation methods for creating and deleting elements?
### Creating elements:
- document.createElement(): Creates a new element.

- element.appendChild(): Adds a new child element to an existing element.

- element.insertBefore(): Inserts a new child before another child.

### Deleting elements:

- element.removeChild(): Removes a child element.

- element.remove(): Removes the element itself.

## Question 10 : What is the this keyword in the context of the DOM?
- ' this ' refers to the element that is the target of the event. For example, if a button triggers an event, ' this ' inside an event listener would refer to the button element.

## Question 11 : How can you handle DOM events?
- element.addEventListener(): Adds an event listener to an element.

- element.removeEventListener(): Removes an event listener from an element.

- Event types include click, keypress, load, input, change, etc.

## Question 12 :  What is the difference between addEventListener and attachEvent?
- addEventListener() is the standard method for attaching events and supports event capturing and bubbling, as well as multiple listeners on the same event.

- attachEvent() is an older method used in Internet Explorer 8 and below and only supports bubbling (not capturing) and doesn't allow multiple listeners.

## Question 13 : What is the document object in the DOM?
- The document object is the entry point for interacting with the DOM. It represents the HTML document and provides methods and properties to access, modify, and manipulate the document's structure, style, and content.

## Question 14 : What is the difference between window and document objects in the DOM?
- window: Represents the browser's window, including the viewport, and provides methods for interacting with the browser itself (e.g., window.alert(), window.location).

- document: Represents the HTML document loaded in the browser and provides methods to interact with the DOM (e.g., document.getElementById()).