
# Dogvacay JavaScript Style Guide() {

*A mostly reasonable approach to JavaScript*
TODO backbone file structure
naming patterns


## Table of Contents


  1. [Naming Conventions](#naming-conventions)
  1. [Variable Declarations](#variable-declaration)
  1. [Whitespace](#whitespace)
  1. [Strings](#strings)
  1. [Numbers](#numbers)
  1. [Calculations](#calculations)
  1. [Importing](#import)


## Notes
We are using the atomic design principal
The design has the following structure
quarks
atom
molecule
orgainsim


The different items in a Sass rule set go in the following order:

Scoped variables
Selector extensions with @extend
Mixin inclusions with @include with the exception of media-query stuff
Regular property: value pairs
Pseudo-class/element nesting with & after an empty line
Regular selector nesting after an empty line
Media query stuff (with or without a mixin)

not plural

## Naming Conventions

**CSS Selectors**
  We are currently using Yandex BEM System for our naming convention

  ````css
  .block { }
  .block--modifier { }
  .block__element { }
  .block__element--modifier { }
  ````

  - Avoid single letter names and acronyms. Be descriptive with your naming.

    ```css
    // bad
    .q {...}

    .btn {...}

    .btn-1 {...}


    // good
    .button {...}

    .button--secondary {...}
    ```

  - Use only lower case variables

    ```css
    // bad
    .Button {...}

    // good
    .button {...}
    ```

  -Use hyphens for a phrase/compound word.

    ```css
    // bad
    .userAnalysis {...}
    .user__analysis {...}
    .user--analysis {...}

    // good
    .user-analysis {...}
    ```

  - You should use a noun or noun phrase as much as possible. `

## Whitespace

  - Use the default spacing in the stylesheet you are working on.  If it is a new file then the default spacing should be 2
  - Ideally, 120-characters wide lines.
  - Use soft tabs set to 2 spaces.

    ```scss
    // bad
    .foo {
    ∙∙∙∙display: block;
    }

    //bad
    .foo {
    ∙display: block;
    }

    //good
    .foo {
    ∙∙display: block;
    }
    ```

  - Place 1 space before the leading brace. (``{``)

    ```scss
    //bad
    .foo{
      display: block;
    }

    //good
    .foo {
      display: block;
    }
    ```

  - Properly written multi-line CSS rules (one rule per line).
     - **Exception**: If there is only one property then the property can be on the same line

    ```scss
    //good
    .foo{
      display: block;
    }

    //better
    .foo {display: block;}
    ```

  - Place at least 1 space before the property value

      ```scss
      //bad
      .foo{
        line-height:$base-line-height;
        display:block;
      }

      //good
      .foo{
        line-height: $base-line-height;
        display: block;
      }

      //better
      .foo{
        line-height: $base-line-height;
        display:     block;
      }
      ```
  - Leave a blank line after blocks and before the next statement

      ```scss
      //bad
      .foo{
        @include padding;
        display:block;
      }
      .fee{
        @include padding;
        display:block;
      }

      //good
      .foo{
        @include padding;

        line-height: $base-line-height;

        display: block;
        color:   green;
      }

      .fee{
        @include padding;

        line-height: $base-line-height;

        display: block;
        color:   green;
      }

      ````
**[⬆ back to top](#table-of-contents)**


## Resources


**Tools**


**Other Styleguides**

  - [EDX Sass & CSS Style Guide](https://github.com/edx/ux-pattern-library/wiki/Styleguide:-Sass-&-CSS)
  - [Current CSS and Sass Styleguide](http://www.sitepoint.com/css-sass-styleguide/)


**[⬆ back to top](#table-of-contents)**

# };
