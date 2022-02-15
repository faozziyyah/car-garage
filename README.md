# carxclusive

A car shop website

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Useful resources](#useful-resources)

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the site depending on their device's screen size
- See the hover states for each cars

### Screenshot

![](images/Screenshot.jpg)
![](images/Screenshot1.jpg)


### Links

- Solution URL: (https://github.com/faozziyyah/car-garage)
- Live Site: (https://faozziyyah.github.io/car-garage/)

## My process

### Built with

- Javascript 
- CSS
- Flexbox

### What I learned

- How to use javascript loops
- Document Object Model

```Javascript
cars.forEach(e => {
    html += `
    <div class="plan col-12 col-sm-3">
    <div class="plan__side plan__side--front">
        <div class="plan__image plan__image--1">
            <img src="images/${e.carImg}.png" class="img-fluid" />
        </div>
        <h4 class="plan__heading plan__heading--1">${e.name}</h4>
        <div class="plan__bullets">
           <p>${e.price}</p>
        </div> 
    </div>
    <div class="plan__side plan__side--back plan__side--back-1"> 
        <div class="plan__button">
            <div class="plan__cost-box">
                <p class="plan__cost-value">${e.price}</p>
            </div>
            <a href="#" class="btn">Shop with us</a>
        </div>
    </div>
</div>
    `

    carsSection.innerHTML = html
});
```
