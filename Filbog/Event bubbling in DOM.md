15-11-2024
events "bubble up", up to the root *document* object. For example, if I have a div with a click event listener that prints "hello div" upon clicking AND a button that prints "hello button" upon clicking that's inside that div, when clicking the div - we'll get "hello div" in the console. But when clicking the button - we'll get both "hello button" and "hello div", in that order. Below, a great video of explaining it and how to turn off that behavior with stopPropagation method.



### Hashtags:


### References (source material, similar notes):
https://www.youtube.com/watch?v=KaHZdW02Tg0&ab_channel=DeeecodeTheWeb