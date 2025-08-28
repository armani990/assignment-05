# assignment-05
1.
=>.getElementById <br>
 -> purpose selects a single element by its id <br>
 -> returns one element and null when if not found <br>
 => .getElementsByClassName <br>
 ->purpose selects all elements with specific class <br>
 -> return a live HtmlCollection of elements. <br>
 --- <br>
=>. querySelector <br>
   ->purpose select elements using any CSS selector <br>
   ->return the first matching element <br>
 =>.  querySelectorAll <br>
   ->purpose select elements using any CSS selector <br>
    -> return all matching elements as static nodelist <br>

 2--<br>
  ->Create the element <br>
  const newDiv = document.createElement("div") <br>
  ->add content or attribute <br>
  newDiv.textContent = "Hello, world!"  <br>
  newDiv.className = "my-class" <br>
 ->choose where to insert it <br>
   const parent = document.getElementById("container") <br>
   parent.appendChild(newDiv) <br>

  3--<br> 
  event bubbling happens when an event on a webpage starts at the target        element and then gradually moves upwards to its parent elements, all the      way to the top of the page <br>
  <div id="parent"> <br>
  <button id="child">Click Me</button> <br>
</div> <br>
if you click the button:- <br>
 -the event triggers on the button first <br>
 -then it moves up to the parent div <br>
 -then to body ,html and finally document. <br>

4 <br> -event delegation in JavaScript is a technique where instead of attaching event listeners to multiple child elements individually, you attach a single event listener to a parent element and use it to handle events for all its children. the event bubbles up from the child element to the parent, where you can determine which child triggered the event. <br>
How it works - <br>
      ->Events in JavaScript bubble up the DOM by default (unless stopPropagation() is used). <br>
      -> we attach a listener to a parent element. <br>
      ->inside the event handler, you check the event.target (the actual element that triggered the event) to see if it matches your              desired child elements. <br>
  Why it is useful:- <br>
   -> Performance: Instead of adding multiple listeners for many child elements, you add only one. <br>
   ->Dynamic elements: Works for elements that are added to the DOM later. <br>
   ->Cleaner code: Reduces repetition and simplifies event handling. <br>

5-- <br>
preventDefault() <br>
  ->purpose to prevent the default action an element from happening <br>
  ->common uses of cases: <br>
                   -preventing a form from submiting <br>
                   -preventing a link <a>from navigation. <br>
                   -stop the browser defaul drag and drop behavaior <br>

stopPropagation() <br>
  ->purpose to stops the event from bubbling up the DOM tree. <br>
   ->common use cases : <br>
            -preventing parent element event handler from being triggered <br>
            -handling an event on a specific element without ancestors. <br>
            
