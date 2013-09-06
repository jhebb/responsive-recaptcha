# Responsive reCAPTCHA

This is a quick theme for <a href="https://www.google.com/recaptcha">reCAPTCHA</a> that makes it friendlier to responsive websites, specifically on mobile interfaces where you might need the captcha narrower than 300px wide.

<img src="http://i.imgur.com/lWuCN.png" alt="Responsive reCAPTCHA screenshot">

## LESS Version

This is a LESS port of https://github.com/chrisvanpatten/responsive-recaptcha -- all orignal design credit goes there. Any changes below are to make the readme relevant for LESS.

The LESS version includes both <a href="https://github.com/JoelSutherland/LESS-Prefixer">Normalize V2</a> and <a href="https://github.com/JoelSutherland/LESS-Prefixer">LESS Prefixer</a>.

## Prerequisites

Here's what you need:

*   You should have reCAPTCHA set up already
*   A LESS compiler, if you want to work with the LESS file. (<a href="http://alphapixels.com/prepros/">Prepos</a>)
*   <a href="http://fortawesome.github.com/Font-Awesome/">Font-Awesome</a> is referenced for the icons (but any icon font, or images, would work)

## Other notes

If you're using an existing reCAPTCHA library, you might want to add the custom HTML to the output function (`recaptcha_get_html` in PHP, for example) to simplify the process of adding reCAPTCHAs.

My original implementation (visible above) used the wonderful <a href="https://github.com/nathansmith/formalize">Formalize</a> from @nathansmith. It's not required and I didn't bundle it here, but I can't recommend it highly enough.

If you want to customize this further and have questions, feel free to ask or consult <a href="https://developers.google.com/recaptcha/docs/customization">Google's documentation</a> on the subject.

## Customising colours

If you're a LESS user, you can customize the colors with some easy included variables. They are:

+ `@recaptcha-base-color`
+ `@recaptcha-border-radius`
+ `@recaptcha-border-radius-inner`
+ `@recaptcha-input-background`
+ `@recaptcha-icons-color`
+ `@recaptcha-icons-shadow`

Simply include these variables before you import `recaptcha.less` and it should use them with no trouble.

Note: the default values are listed in `recaptcha.less`, in the "Settings" section.

## Caution

**Use wisely.** I don't have a `min-width` set on the captcha, and if you're not careful the captcha could get too small to read! Make sure you test thoroughly on various devices at various widths to make sure that won't be an issue.

## Unlicense

This is free and unencumbered software released into the public domain.

Anyone is free to copy, modify, publish, use, compile, sell, or
distribute this software, either in source code form or as a compiled
binary, for any purpose, commercial or non-commercial, and by any
means.

In jurisdictions that recognize copyright laws, the author or authors
of this software dedicate any and all copyright interest in the
software to the public domain. We make this dedication for the benefit
of the public at large and to the detriment of our heirs and
successors. We intend this dedication to be an overt act of
relinquishment in perpetuity of all present and future rights to this
software under copyright law.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
IN NO EVENT SHALL THE AUTHORS BE LIABLE FOR ANY CLAIM, DAMAGES OR
OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
OTHER DEALINGS IN THE SOFTWARE.

For more information, please refer to <http://unlicense.org/>
