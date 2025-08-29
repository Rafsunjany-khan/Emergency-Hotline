1. What is the difference between getElementById, getElementsByClassName, and querySelector / querySelectorAll?
Solution:
getElementById - Return a single unique element.
getElementsByClassName - Used HTML collection list items or multiple element
querySelector - When need one element that match a CSS selector.
querySelectorAll - When need all elements matching a CSS selector.

2. How do you create and insert a new element into the DOM?
Solution: 
const cardElement = document.createElement('div');
document.body.appendChild(cardElement);

3. What is Event Bubbling and how does it work?
Solution:
when you click a button event happend on that specific element then its parents this
is called event bubbling.

<button id="child">click me</button>
<div id="parent"></div>
<script>
document.getElementById('child').addEventListener('click', () => alert('Button clicked!'));
document.getElementById('parent').addEventListener('click', () => alert('Div clicked!'));
</script>

4. What is Event Delegation in JavaScript? Why is it useful?
Solution:
Event Delegation used for single event listener added to a parent element instead
of children element. The parent handel children using event bubble.

useful because Reduces memory usage by using fewer event listeners.Works for dynamically
added elements and code easy maintains.

5. What is the difference between preventDefault() and stopPropagation() methods?
Solution:
preventDefault() - stop default action
stopPropagation() - stop event from moving up or down the DOM.