## Gutenberg HTML and CSS Notes

In the html in several places I added multiple divs
```html
<div class="x-header">
    <div class="content">
    ---- Place Content In between ----
    </div>
</div>

<div class="x-top-level">
    <div class="content">
    ---- Place Content In between ----
    </div>
</div>
```
The purpose of this was to add differing colors for sections of the page to add border and background colors and stylistic margins.

I also added a `link` tag to each html page pointing to the `makeitlooknice.css` stylesheet to apply all custom css I wanted to apply.

Stylistic CSS choices:
- Generally I find that it is easier to view dark content for longer periods of time so I opted for a darker color palette.
- To provide focus on the certain sections of the page I used contrast.
    - The html tag background is grey so it is out of focus
    - the blue is a bit brighter to indicate general position to view the content
    - The white borders signify a section that contains relevant context. Which in this case is the actual book, so that is given the most focus
    - h2 tags signifiy titles or chapter changes, so to make it easier to scroll and recognize changing chapters I made h2 tags white so chapter counts can be performed easily.
    - In doc3 in the html there were some margin changes related to the `.toc` class which I had to remove in order for my css to take effect. This is because my CSS was element based, which has less priority than a class css property.