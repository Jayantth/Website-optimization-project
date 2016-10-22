# Guidelines

- The source code is in the website-optimization-project repositary.[https://github.com/Jayantth/Website-optimization-project.git]
- Run the index.html from main directory.
- Used github pages to host index.html on server for testing on Pagespeed Insights.Please use this link for testing the speed.[https://jayantth.github.io/Website-optimization-project/]


## Optimizations made to index.html:

- Style css made internal rather than external.
- Media="print" added for print.css.
- Optimized jpeg files img/profilepic.jpg and views/images/pizzeria.jpg.
- Set the JS files to async.
- Moved all js files to bottom of <body>.

## For achieving 60fps:

- Made items and itemLength as global variable and defined it outside updatePositions().
- Moved few variables outside for loop in updatePositions().
- Used style.transform property instead of style.left property.
- Number of pizzas in background is calculated according to the screen height.
- Replaced querySelector by getElement method.
- Modified the .mover class in CSS file.

## For resizing pizza within 5ms:

- Replaced querySelector by getElement method.
- Optimized switch function to directly change the width in changePizzaSizes() function.