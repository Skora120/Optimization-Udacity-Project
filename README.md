# Project: Website Optimization for [Udacity](https://udacity.com)

I was provided with poorly optimalizated website and my job was to make `index.html` getting over 90 points on Google Insights and `pizza.html` running on 60fps and also optimalizate function of resize pizzas.

Github repository contains two versions of sites one of them is in catalog `src` and it is that one with poor optimization another one is `dist` and this one is fully optimizated.

### Links to github.io
* #### [Unoptimizated Page](https://skora120.github.io/Optimization-Udacity-Project/src/)

* #### [Optimizated Page](https://skora120.github.io/Optimization-Udacity-Project/dist/)

## How to run?

1. Download zip file from GIT.
2. Unzip it somewhere on your desktop.
3. Run `index.html` in catalog `dist`(or src for first version) in browser(Recommended Google Chrome).

## Optimization steps
##### Index.html
* Inline compressed css
* async scripts
* inline scripts
* compressed images

##### Main.js
Changed function `updatePositions` by:
* create global var `items` to decrease amount of work for browser also used `document.getElemtsByClassName` insted of `document.querySelectorAll`
* create one more for loop to iterate for each unique vlues
* create array `phaseArr` for "scroll values"

Changed function `changePizzzaSizes` by:
* create var `radomPizzaElem` for getting elemtns of `randomPizzaContainer` class by using `document.getElemntsByClassName`
* get all posible values from for loop for increse speed
* rebuild function using created before var `radomPizzaElem`

##### Pizzeria site
I optimizated `pizza.html` with simillar methods to `index.html`.

## Screen from Google Insights of `index.html`

![Desktop](https://d3higte790sj35.cloudfront.net/images/wv/kc/b5660a138662d25a90093371444740d6.jpeg)
![Mobile](https://d3higte790sj35.cloudfront.net/images/ru/rf/0d3219238785ad41a55c9dd4daa8061d.jpeg)