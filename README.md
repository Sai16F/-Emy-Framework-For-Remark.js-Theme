----
## Welcome to Emy-Framework For Remark.js Theme with Markdown Structure for slideshow layouts.
## ALL RIGHTS RESERVED FOR THE DEVELOPER ON THIS FRAMEWORK PROJECT AND ITS FILES.

# This is the way you are going to use this Framework style sheet with your Remark Theme:
- Actually, I've build This Framework to work with Specified 9 layouts. But also, Its Grid System will give you the ability to build any layout Design you want.
- But first: There are some rules you should follow to work with this Framework with Your Remrak.js Theme and the Markdown Structure.

---
1. link the framework css file into your HTML page at the end of the "head" tag.

```html
<head>
    <title>9 Layouts</title>
    <meta http-equiv="Content-Type" content="text/html; charset=UTF-8"/>
    <style type="text/css">
      @import url(https://fonts.googleapis.com/css?family=Yanone+Kaffeesatz);
      @import url(https://fonts.googleapis.com/css?family=Droid+Serif:400,700,400italic);
      @import url(https://fonts.googleapis.com/css?family=Ubuntu+Mono:400,700,400italic);

      body { font-family: 'Droid Serif'; }
      h1, h2, h3 {
        font-family: 'Yanone Kaffeesatz';
        font-weight: normal;
      }
      .remark-code, .remark-inline-code { font-family: 'Ubuntu Mono'; }
    </style>
    <link rel="stylesheet" href="emy-framework.css">
  </head>
```
---
2. To use one of the 9 layouts: Use The specific Markdown Structures and the specific classes which for each layout as you see, to make any of the 9 layouts which were provided in the framework is working as planned.
```markdown
class: intro

.w-12[
  # Title
  ## Subtitle
]

---
class: image-up

.h-10[
  ![image](horizontal.jpg)
]
.h-2.p-2[
  ## Image With Caption 
]

---
class: full-screen-padded

.w-12[
  # One Column Layout
  * Unordered list can use asterisks
  - Or minuses
  + Or pluses
  * Lorem ipsum dolor sit amet, consectetur adipiscing elit.
  * Lorem ipsum dolor sit amet, consectetur adipiscing elit.
  * Lorem ipsum dolor sit amet, consectetur adipiscing elit.
]

---
class: image-down
.h-8.padded[
  # One Column Layout And Full-Width image
  * Lorem ipsum dolor sit amet, consectetur adipiscing elit.
  * Lorem ipsum dolor sit amet, consectetur adipiscing elit.
  * Lorem ipsum dolor sit amet, consectetur adipiscing elit.
]
.h-4[
  ![image](horizontal.jpg)
]

---
class: two-col-padded
.w-12[
  # Two-Column Layout
]
.w-6.h-12[
* Lorem ipsum dolor sit amet, consectetur adipiscing elit.
* Lorem ipsum dolor sit amet, consectetur adipiscing elit.
* Lorem ipsum dolor sit amet, consectetur adipiscing elit.
]
.w-6.h-6.img-cover[
  ![image](horizontal.jpg)
]

---
class: three-col-padded
.w-12[
  # Three-Column Layout
]
.w-4[
* Lorem ipsum dolor sit amet, consectetur adipiscing elit.
* Lorem ipsum dolor sit amet, consectetur adipiscing elit.
* Lorem ipsum dolor sit amet, consectetur adipiscing elit.
]
.w-4[
* Lorem ipsum dolor sit amet, consectetur adipiscing elit.
* Lorem ipsum dolor sit amet, consectetur adipiscing elit.
* Lorem ipsum dolor sit amet, consectetur adipiscing elit.
]
.w-4[
* Lorem ipsum dolor sit amet, consectetur adipiscing elit.
* Lorem ipsum dolor sit amet, consectetur adipiscing elit.
* Lorem ipsum dolor sit amet, consectetur adipiscing elit.
]

---
class:  image-right
.w-8.padded[
  # Image-Right
  * Lorem ipsum dolor sit amet, consectetur adipiscing elit.
  * Lorem ipsum dolor sit amet, consectetur adipiscing elit.
  * Lorem ipsum dolor sit amet, consectetur adipiscing elit.
]
.w-4.img-cover[
  ![image](vertical.jpg)
]

---
class:  image-left
.w-4.img-cover[
  ![image](vertical.jpg)
]
.w-8.padded[
  # Image-Left
  * Lorem ipsum dolor sit amet, consectetur adipiscing elit.
  * Lorem ipsum dolor sit amet, consectetur adipiscing elit.
  * Lorem ipsum dolor sit amet, consectetur adipiscing elit.
]

---
class: image-show
.w-8.h-12.img-cover[
  ![image](tree.jpg)
]
.w-4.h-12[
  .h-6.img-cover[
    ![image](com-ver.jpg)
  ]
  .h-6.img-cover[
    ![image](horizontal.jpg)
  ]
]
```
---
3. The Grid System of Emy-Framework was built on making the gird rows and columns are under the control of the user, for Example:
* After you give your slide the class name: "container" you can do something like:
  - Controle your content place by the vertical and horizontal units of Emy-Framework classes in Grid System.
  - Each of Vertical and Horizontal has 12 units, the 12 uints are separated equally by percentage value(%) = 8.33333% for each unit.
  - For Example: 
   - The ".w-12" class meaning that: the div will take 12 units of the total 12 units = 100% width.
   - The ".w-4" class meaning that: the div will take 4 units of the total 12 units = 33.3333% width from the total width ot its parent container which itself has 100% in width and height.
   - The ".h-6" class meaning that: the div will take 12 units of the total 12 units = 50% height from the total height ot its parent container which itself has 100% in width and height.
   - The ".h-3" class meaning that: the div will take 4 units of the total 12 units = 25% height from the total height ot its parent container which itself has 100% in width and height.
  - Specify specific row with width and height at one by one class name. like using ".w-5-h-4" for making div with 41.6666% width and 33.3333% height from the total width and height ot its parent container which itself has 100% in width and height. but make sure you put the width first in the class name.
