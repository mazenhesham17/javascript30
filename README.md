# javascript30
My notes for Wes Bos javascript30 course

## Day 1
Task: Adding some styling interactions with the keyboard press

Introducing the **dataset** concept in which is an object in each HTML element which can hold custom variables to use later.

Example:
```HTML
<audio data-key="65" src="sounds/clap.wav"></audio>
```
Accesing the data object in javascript:
```JS
/* select the element by the key variable */
const element = document.querySelector('audio[data-key="65"]') ;
console.log(element.dataset.key) ; /* 65 */
```

## Day 2
Task: Adding interaction to analog clock

Introducing the **setInterval** function in javascript, calls a function at specified intervals (in milliseconds).

Example:
```JS
/* calls setDate function every second */
setInterval(setDate, 1000);
```

## Day 3 
Task: Changing color, blur, padding using the HTML input elements 

Introducing **variables in CSS**.
example:
```css
/* initialize variable */
:root{
  --blur: 10px;
}

/* access the variable */
img{
  filter: blur(var(--blur));
}
```

Update variable using javascript:
```JS
document.documentElement.style.setProperty("--blur","20px") ;
```
