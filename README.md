### What was the project about?

The project is part of the 50 Projects in 50 Days with Brad Travesy via Udemy. The course is a code-a-long to further cement skills used within HTML, CSS, and Vanilla JavaScript.

This particular project introduced a scrolling animation effect. The idea being, as the user scrolls down the webpage, content emerges from either the left or right side of the screen.

[Scrolling Animation](https://totallysly.github.io/406.-50PROJECTS50DAYS--scrolling-animation/)

#### CSS

Again, this was a rather simple CSS project which did not introduce any new skills. It did introduce the logic behind the scrolling content. By using the `translateX( )` property and offsetting the content by 400%. This takes the content off the screen along the X axis and will reappear when scrolling with an animation effect and JavaScript as the user scrolls down the webpage.

Also, to create the effect of the content entering from alternate sides, the psuedo-element `nth-of-type(even)`

#### JavaScript

The JavaScript itself was rather simple, however there was a mathematical calculation that was not explained that required some research.

    const  triggerBottom = (window.innerHeight / 5) * 4

There was no explanation as to how this calculation was made, and the only assumption I can make is that it was solved via trial and error.

However, the logic is using the innerHeight method on the window and trying to calculate at which window height should the content animation appear from the left or right. The calculation given gives 0.8 - or 80% So when the user scrolls down, when the window height is at 80%, the content will appear from either the left or right hand side.

[windows.innerHeight Diagram](https://postimg.cc/jDR7xptM)

_Credit goes to Excel for the diagram. This was taken from under the lecture notes on the 50 Projects in 50 Days - HTML, CSS, Vanila JS - Brad Travesy Udemy Course._

The tutorial introduced [element.getBoundingClientReact( )](https://developer.mozilla.org/en-US/docs/Web/API/Element/getBoundingClientRect)

This is still quite tricky for me to understand. I am at the stage of understanding the theory, but I am not sure if I can put it into action as of yet. I have watched several YouTube videos to help my understanding with [# getBoundingClientRect() in Javascript DOM - dcode](https://www.youtube.com/watch?v=MKpZadkuT-0) giving a rather straight forward explanation.

At a basic level, it can be used to change the UI as a user scrolls down a webpage. The `getBoundingClientRect()` method is great for finding a placement of an element and using the sizing to manipulate said element.

> Written with [StackEdit](https://stackedit.io/).
