# JavaScript-guide

## ..Link js to html
1. before finishing body :
```
<script src="app.js"></script>
```
## ..Starting code 
alias: `clg`
```
console.log("hello this s js")
```
--you can see it in CONSOLE DEV TOOLS
## ..Selecting items
`const` item = document.querySelector("alias")
```
const wrapper = document.querySelector(".slider-wrapper")

console.log(wrapper)
```
## ..Funtions
#_background color

`style`.`backgroudColor`
```
wrapper.style.backgroundColor="red"
```
#_change position
`transform`
```
wrapper.style.transform = "translateX(-100vw)"
```
#_ when click slide
 `querySelectorAll` `forEach(item, index)`
```
const wrapper = document.querySelector(".slider-wrapper");
const menuItems = document.querySelectorAll(".menu-item");

menuItems.forEach((item,index) => {
    item.addEventListener("click", () => {
        wrapper.style.transform = `translateX(${-100 * index}vw)`;
    });
});
```
