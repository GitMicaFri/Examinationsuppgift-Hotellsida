<!DOCTYPE html>
<html>
<head>
<style>
body {
  background-color: tan;
  color: black;
}

<!--On screens that are 992px wide or less, the background color is blue -->
@media screen and (max-width: 992px) {
  body {
    background-color: blue;
    color: white;
  }
}

<!--On screens that are 600px wide or less, the background color is olive--->
@media screen and (max-width: 600px) {
  body {
    background-color: olive;
    color: white;
  }
}
</style>
</head>
<body>

<h1>Resize the browser window to see the effect!</h1>
<p>By default, the background color of the document is "tan". If the screen size is 992px or less, the color will change to "blue". If it is 600px or less, it will change to "olive".</p>

</body>
</html>

<!-----Exempel från ChatGPT--------->
Creating responsive web designs for both desktop and mobile screens involves using CSS media queries to apply styles based on the screen size or device characteristics. Here's a basic structure for writing media queries in a stylesheet:

css
Copy code
/* Default styles for all screen sizes */
/* These styles apply to screens of all sizes */

body {
    font-size: 16px;
    /* Other default styles */
}

header {
    background-color: #333;
    color: #fff;
    /* Other header styles */
}

/* Media query for screens with a maximum width of 768px (typical for tablets and small screens) */
@media (max-width: 768px) {
    body {
        font-size: 14px;
        /* Adjust styles for smaller screens */
    }

    header {
        padding: 10px;
        /* Modify header styles for smaller screens */
    }

    /* Add styles specific to tablet and smaller screens */
}

/* Media query for screens with a maximum width of 480px (typical for mobile phones) */
@media (max-width: 480px) {
    body {
        font-size: 12px;
        /* Further adjust styles for smaller screens */
    }

    header {
        padding: 5px;
        /* Modify header styles for mobile screens */
    }

    /* Add styles specific to mobile screens */
}
In this example:

Default styles are applied to all screen sizes.
Media queries are used to target specific screen widths.
The max-width property in the media query indicates that the enclosed styles will be applied when the screen width is equal to or smaller than the specified value.
You can add as many media queries as needed to handle different screen sizes and orientations. The key is to adjust the CSS rules within each media query to create a responsive layout and design that works well on various devices.

Remember to test your responsive design on real devices and browsers to ensure it functions correctly and looks good on all screen sizes. Additionally, consider using flexible layouts, such as using percentage-based widths and relative units like em and rem, to make your design more adaptable to different screen sizes.
