# Custom Class Styling

Here are some examples for the adheared styling for the Monmouth-Independence Visitor Center website. Below are some elements that have been altered from the basic / Bootstrap styling and how to access these elements through classes.

## Quick Links
- [Font](#font)
- [Headings](#headings)
- [Text](#text)
- [Forms](#forms)
- [Buttons](#buttons)
- [Color Scheme](#color-scheme)

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

When there needs to be a style for a specific heading, team should default to inline styling for given heading. An example for specific inline heading styles could be

```html
<h1 style='font-weight: [selected-weight]; font-style: [selected-style]'> Heading </h1>
```

> `selected-weight` could include 100, 300, 400, 500, 700 as these are the font-weights that are currently imported from Google Fonts. Since the imported font supports italic, this can be used for `selected-style` if needed.

Below is an example of 'Roboto' font for each heading element

![](https://i.imgur.com/lQzSv40.png)

## Text

Similarly, text elements such as `<p>, <label>, <button>` will adhere to using the imported font 'Noto Sans JP'. This should create a cohesive feel to the website that allows for easy viewing on desktop / mobile devices. Although, should the font fail to be imported through the stylesheet link, the selected font to replace will be sans-serif.

> Nothing needs to be done for the team to adhere to this guidline as the font is selected to be used for the elements listed above preemptively.

Below is an example of 'Noto Sans JP' font for a text element

![](https://i.imgur.com/9iFeA66.png)

## Forms

Forms will use Bootstrap's implementation along with slight modifications to allow the website to have a cohesiev design. Below is am example of a forms implementation and code.

> Nothing needs to be done for the team to adhere to this guidline as the form element is styled to be used for the website directly.

![](https://i.imgur.com/TmBA2Ah.png)

```html
<form>
    <div class="form-group">
        <label for="inputEmail4">Email</label>
        <input type="email" class="form-control" id="inputEmail4">
    </div>
    <div class="form-group">
        <label for="inputPassword4">Password</label>
        <input type="password" class="form-control" id="inputPassword4">
    </div>
    <div class="form-group">
        <label for="inputAddress">Address</label>
        <input type="text" class="form-control" id="inputAddress" placeholder="1234 Main St">
    </div>
    <button type="submit" class="btn btn-submit">Sign in</button>
</form>
```

Note that if form grid needs to be altered to allow for fields on the same row using Bootstrap's layout, an example is provided below.

![](https://i.imgur.com/nZxA1tZ.png)

```html
<form>
    <div class="form-row">
        <div class="form-group col-md-6">
            <label for="inputEmail4">Email</label>
            <input type="email" class="form-control" id="inputEmail4" aria-describedby="emailHelp">
            <small id="emailHelp" class="form-text text-muted">Email description</small>
        </div>
        <div class="form-group col-md-6">
            <label for="inputPassword4">Password</label>
            <input type="password" class="form-control" id="inputPassword4" aria-describedby="passHelp">
            <small id="passHelp" class="form-text text-muted">Password criteria</small>
        </div>
    </div>
    <div class="form-group">
        <label for="inputAddress">Address</label>
        <input type="text" class="form-control" id="inputAddress" placeholder="1234 Main St">
    </div>
    <button type="submit" class="btn btn-submit btn-light">Sign in</button>
</form>
```

Note that if there needs to be a short description for a specific field, the `<small>` element may be appended. 

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
The initial color theme for the website can be viewed below. Elements such as `<button>` and `<form>` have already been created to adhere to this color scheme.

![](https://i.imgur.com/PqPICq8.png)

> Note that this custom styling is subject to change as progress is made to the website and feedback is received from the stakeholders.
