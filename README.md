# CNY 2023
Basically a series of divs that are transformed when their parent div is moused over. The transformations are revsered on mouseout.

## HTML/CSS
- a div with id `container`. On mouseover, `doChange()` is called. On mouseout, `revserseChange()` is called.
- 5 divs with class `shading`, each with its own id. The ids are just for styling because we are trying to avoid embedding the styles in HTML. Just a matter of preference, nthing more.
- 4 divs with class `number`. The `position` property is set to `absolute`. And then in the HTML, we embed the `margin-left` and `margin-top` properties.
- 2 divs with the class `text`. They will not both be visible at the same time.

## JavaScript
- `doChange()` does the following
1. Fades out the instructional text and fades in the greeting (class `text`).
2. Translates each `number` div. Then scale and rotate accordingly. (the order is important!)
3. Fades in `shading` divs.

- `reverseChange() does the opposite!
1. Fades in the instructional text and fades out the greeting (class `text`).
2. Set all translation properties of `number` divs to 0. All scaling transformations are reset to 1, and rotations are reset to 0.
3. Fades out `shading` divs.
