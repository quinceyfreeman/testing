# Styling Conventions

Here are some examples for the adheared styling for the Monmouth-Independence Visitor Center website. Below are some elements that have been altered from the basic / Bootstrap styling and how to access these elements through classes.

## Font
DF has decided to select a modern font that users of the website will see across all pages. The font selected to be used for the website is 'Roboto'. This font is found on [Google Font](https://fonts.google.com/specimen/Roboto?preview.text_type=custom) and is imported into the website using a stylesheet link in `Shared/_Layout.cshtml`. Below is an example of the font.

![](https://i.imgur.com/rliYuik.png)

## Headings
Headings will use the 'Roboto' font as described above and can be accessed using the related tags `(h1,..,h6)`. Note that when using Bootstrap's header classes e.g. 
```html
<h1 class='display-#'></h1>
```
 these classes take precedence over DF custom classes. When making headings, team should default to use basic heading elements.

### Header Styling

When there needs to be a style for a specific heading, team should use default to inline styling for given heading. Some examples for specific inline heading styles could be

```html
<h1 style='font-weight: [selected-weight]; font-style: [selected-style]'> Heading </h1>
```

> `selected-weight` could include 100, 300, 400, 500, 700 as these are the font-weights that are currently imported from Google Fonts. Since the imported font supports italic, this can be used for `selected-style` if needed.

## Text

Similarly, text elements such as `<p>, <label>, <button>` will also adhere to using the 'Roboto' font. This should create a cohesive feel to the website that allows for easy viewing on desktop / mobile devices. Although, should the font fail to be imported through the stylesheet link, the selected font to replace will be sans-serif.

> Nothing needs to be done for the team to adhere to this guidline as the font is selected to be used for the elements listed above preemptively.

## Forms

## Buttons
Buttons can be any of the below options. Implementing these custom buttons will follow Bootstrap's formula for making a button.

<p align="center">
  <img src="https://media.giphy.com/media/J7vDfUK5UeYIhRsxZx/giphy.gif">
</p>

Calling these buttons can be done by using the following:

```html
<button type="button" class="btn btn-submit">Submit</button>
<button type="button" class="btn btn-blue">Blue</button>
<button type="button" class="btn btn-orange">Orange</button>
<button type="button" class="btn btn-grey">Grey</button>
```

## Color Scheme
The initial color theme for the website can be viewed below. 

![](https://i.imgur.com/PqPICq8.png)
