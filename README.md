# css-sticky-footer
CSS sticky footer using CSS table layout

## Description
So you want a CSS sticky footer, the kind that makes the footer stay at the bottom of a page when there's not enough content. This code will solve that.

You basically want this:
![alt tag](https://raw.githubusercontent.com/oscarmakesstuff/css-sticky-footer/master/readme_bits/example2.png)

And not this:
![alt tag](https://raw.githubusercontent.com/oscarmakesstuff/css-sticky-footer/master/readme_bits/example1.png)

## How it works
This uses a cleverly old trick back when the web was built using tables. Of course, that was then. A more modern version would be to use CSS table layout. It sets your `<body>` as a table and the parent elements of your content containers as a table-row with the `<main>` being your main body of content and setting that to height: 100% pushes the footer to the bottom.

## Notes
IE/Edge may have a rendering issue where the elements are not filled properly by the CSS background property when there are anchor tags present in the container. You could try wrap the container in another container and set that to display: table-cell and apply the background to that instead.
