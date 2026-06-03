Header and Footer Use Documentation
===================================

This document describes the files included with the U of M header/footer and the general process for updating your site.

For information, guidelines, and additional header/footer options [visit the University Relations Brand Site](https://university-relations.umn.edu/resources/web-header-and-footer-download).

Files
-----

Your header/footer download package will contain the following files:

*   **README.html and documentation.html**—General documentation and use instructions. Delete these files before you publish your site.
*   **2022-tc.html**—Your generated template.
*   **/css/**—Contains the generated CSS for your template as well a stylesheet to support IE8
*   **/img/**—Contains sprites for the Twin Cities wordmark and other elements. Contains retina (@2x) versions of each sprite.
*   **/js/**—Contains two files. `html5shiv.printshiv.js` enables the use of HTML5 elements in IE. [Read more about The HTML5 Shiv if you are interested](https://github.com/aFarkas/html5shiv). The `umnhf-2015.js` file supports collapsible menus on small screens, auto-updating of the copyright date, etc.

Use
---

1.  Copy the header and footer code from `2022-tc.html` into your site template. This file contains various comments. Review them and take any appropriate actions. Remove comments before moving the template to a public-facing site. Your unit-specific content will go in: `<main id="umn-main" role="main"> </main>`
2.  Move the css, img, and js folders into the root directory of your site.
3.  Verify that everything displays correctly at all screen widths.

Additional Customization
------------------------

If you decide at a later date that you would like to include an element in your header or footer that you did not originally include you must complete the Template Builder form again to download a new set of template files.

After you have done this, copy the HTML from the missing section to your template and add the newly generated CSS file to your site.

Questions/Troubleshooting
-------------------------

If you have questions or need assistance please contact [urweb@umn.edu](mailto:urweb@umn.edu).
