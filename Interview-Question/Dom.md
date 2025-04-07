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

## Question 5 : How do you select elements using the DOM?
- Elements can be selected using various DOM methods :
- document.getElementById(): Selects an element by its id.

- document.getElementsByClassName(): Selects elements by their class name.

- document.getElementsByTagName(): Selects elements by their tag name.

- document.querySelector(): Selects the first matching element based on a CSS selector.

- document.querySelectorAll(): Selects all matching elements based on a CSS selector.
