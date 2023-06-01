# Convert pixel to REM with CSS variables

Now your page will have better accessibility😄

## References

> W3Schools (Accessibility text size)

```sh
https://www.w3schools.com/accessibility/accessibility_text_size.php
```

> Convert PX to REM with CSS variables

```sh
https://coryrylan.com/blog/converting-css-pixels-to-rems
```

## (CSS) Add this to your stylesheet

```css
/* 
  > Convert PX to REM with CSS variables
    >> Reference: https://coryrylan.com/blog/converting-css-pixels-to-rems
*/

:root {
  /* PX TO REM */
  --px-base: 16;
  --px-to-rem: 1rem;

  /* PX TO REM: 2-10 */
  --px-2: calc(2 / var(--px-base) * var(--px-to-rem));
  --px-4: calc(4 / var(--px-base) * var(--px-to-rem));
  --px-6: calc(6 / var(--px-base) * var(--px-to-rem));
  --px-8: calc(8 / var(--px-base) * var(--px-to-rem));
  --px-10: calc(10 / var(--px-base) * var(--px-to-rem));
  
  /* PX TO REM: 12-20 */
  --px-12: calc(12 / var(--px-base) * var(--px-to-rem));
  --px-14: calc(14 / var(--px-base) * var(--px-to-rem));
  --px-16: calc(16 / var(--px-base) * var(--px-to-rem));
  --px-18: calc(18 / var(--px-base) * var(--px-to-rem));
  --px-20: calc(20 / var(--px-base) * var(--px-to-rem));
}

/* 
  > BEM Methodology (Custom)
    >> .header
      >>> .header__nav
        >>>> .header__nav-list
          >>>>> .header__nav-list-li
            >>>>>> .header__nav-list-li-a 
*/

.header__nav-list-li-a {
  font-size: var(--px-20); /* PX to REM */
}
```

## (HTML) Add this in the body of your page

```html
<header class="header">
  <nav class="header__nav">
    <ul class="header__nav-list">
      <li class="header__nav-list-li">
        <a class="header__nav-list-li-a" href="#">Hello Accessibility!</a>
      </li>
    </ul>
  </nav>
</header>
```

## More details

- Check out this style sheet: [px-to-rem.css](https://github.com/flaubert-dev/px-to-rem-css-variables/blob/main/px-to-rem.css)
- Check out this HTML document: [px-to-rem.html](https://github.com/flaubert-dev/px-to-rem-css-variables/blob/main/px-to-rem.html)
