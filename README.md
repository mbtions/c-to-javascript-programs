# c-to-javascript-programs
Equivalent codes of C programs in JavaScript

## DOM
### What is DOM?
DOM stands for **Document Object Model**. It is a programming interface that allows us to create, change, or remove elements from the document. We can also add events to these elements to make our page more dynamic. The DOM views an HTML document as a tree of nodes

### Four Pillars of DOM
1. Selection of an Element
2. Changing HTML
3. Changing CSS
4. Event Listener

### 1. Selection of an element
**How to select an element using DOM?**
using the document object 
document.querySelector("h1")  => It selects the heading 1 tag h1 if it is present in the HTML. 
- HTML Element => document.querySelector("tagname");
- Class Selection => document.querySelector(".classname");
- Id Selection => document.querySelector("#id-name");

  ### 2. Changing HTML
  innerHTML function is used to manipulate the HTML associated to the selected HTML element.
  *Ex:* var a = document.querySelector("h1")
  a.innerHTML = "Text Changed"

  ### 3. Changing CSS
  style object is used to change the styling of the selected HTML element.
  *Ex:* var para = document.querySelector("p")
  para.style.backgroundColor = "red";

  *NOTE: the css properties are here in the camelCase form.*
  Ex: background-color: red; => backgroundColor ="red";

  ### 4. Event Listener
  *So what is **event**?* Something that is happening or takes place.  
  And what is **Listener**? Observer or Someone who is paying attention towards something.

  Therefore, Event Listener is the observer who is paying attention towards all the events happening.

      document.querySelector("h1");
      // this addEventListener is a Higher Order Function and it takes two properties as arguments,
      // first one is the name of the event (click, drag, longPress, etc) and
      // other one is a function which is to be performed on this event encounter.
      a.addEventListener("click", function() {
          console.log("Clicked H1 element!");
      });

  
  
  
  

