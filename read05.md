# Reading Notes 05

## What is CSS?

CSS stands for Cascading style sheets. It is a programming language used to give color, animation, and style to html sheets.

- The key to understanding how CSS works is to imagine that there is an invisible box around every HTML element
- CSS creates rules that control the way that each individual box (and the content of that box) are presented.
- CSS works by associating rules with HTML elements. CSS rules contain two parts: a *selector* and a *declaration
- Selectors indicate which element the rule applies to. You can apply the same rule to more than one element by seperating the element names with commas.
- Declarations indicate how elements referred to in the selector should be styled. Declarations are split into two parts, (property, and value) that are seperated by a colon ;
- You can use CSS rules in an html document if you surround them in a *style* element

### How to specify color

You can specify any color in CSS in one of three ways

- *RGB Values* (express colors in terms of how much red green and blue are used to make it up)

- *Hex Codes*  (6 digit codes that represent how much red blue and green are being used preceded by a hashtag)

- *Color Names* (147 predefined colors ex: darkblue)

__*CSS3 introduces hsl color property*__

- This allows you to change color using *hue* *saturation* and *lightness*
- Hue is expressed as an angle (0 - 360 degrees)
- Saturation is expressed as a percentage (0 - 100)
- Lightness is expressed as a percentage (0% being white, 50% being normal, 100% being black)

- You can also change the opacity by using the opacity property (values range from 0.0 to 1.0)
