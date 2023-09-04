# javascript30
My notes for Wes Bos javascript30 course

## Day 1
Task: Adding some styling interactions with the keyboard press

Introducing the **dataset** concept in which is an object in each HTML element which can hold custom variables to use later

example:
```HTML
<div data-key="65" class="key">
  <kbd>A</kbd>
  <span class="sound">clap</span>
</div>
```
Accesing the data object in javascript:
```JS
/* select the element by the key variable */
const element = document.querySelector('audio[data-key="65"]') ;
console.log(element.dataset.key) ; /* 65 */
```

## Day 2
Task: Adding interaction to analog clock

Introducing the setInterval function in javascript, calls a function at specified intervals (in milliseconds).

example:
```JS
/* calls setDate function every second */
setInterval(setDate, 1000);
```
