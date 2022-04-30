# Author:- Vansh Baghel

# Date:- 19-April-2022

# Email :- vanshbaghel912@gmail.com

# Linkedin :- https://www.linkedin.com/in/vansh-baghel-24ab42232

# Feel free to contact me if you face any queries or errors.

# How to search any text in a big documentation:-

- Press (Ctrl+F) and get the text which you want instantly rather than searching it manually.

# Properties in CSS :-

### Syntax

Property:Values

EG:- color:green

## Link of CSS into HTML:-

3 ways :-

### a) **Inline**:- `<tagname style="property:value;">`

- This is preffered to be use where we need some only minute change in the element.

### b) **External**:-

- Can create new file of css and then link it to html.

* This is preffered to be used when we have many lines of codes to decorate our web page.

* This is most commonly used by me bcoz it lets the html file look like html more rather than more of a style related file.

- Code to link:-
  `<link rel="stylesheet" href="Filename.css"> `

### c) **Internal**:-

`<style>` properties `</style>`

- Here we make style wala tag and add properties into the tags we need in that same html file itself.

- This doesnt require to make any external file for styling.

## Selectors in CSS:-

CSS selectors are used to **find** (or select) the HTML elements you want to style.

```Css
Syntax:- h1 {property:value;}
```

### Types of selectors:-

#### 1. **Combined selectors**:-

We write all the elements we want to change with ","

#### 2. **Type selector**:-

We just write the element name.

#### 3. **Class selector**:-

` <h1 class="className"> .className{}`

#### 4. **ID selector**:-

Same as class, just replace with word id and .className with #idName 5.**Attribute selector**:- We write attribute into sq bracket & then curly braces.

#### 5. **Pseudo-class selectors** :-

```CSS
 Syntax:- ElementName:pseudo-class{}
```

#### 6. **Attribute selector**:-

We write attribute into sq bracket & then curly braces.

> Some imp selectors:- hover,visited,link,float,hidden.

#### 7. **Pseudo-elements selectors**:-

select and style a part of an element & change that particular part.

#### 8. **Combinator selectors**:-

Select elements based on a specific relationship between them ie child element ko select krta h.

```CSS
 Syntax:- article > (tagElement) {}
```

#### 9. **Universal selector**:-

Used to select all elements from a file.

Syntax:- \\\* {} <!--Here we added \ to ignore the further \ -->

#### 10. **\- wala method**:-

If there are 3 para after h1 and u want to make changes only in 3rd para then u can write (h1+p+p+p){}.

- To give color to specific tags in full file:-
  `p,a { color: green;}`

- To give class ke liye :- `i.idk{color: blue;}` --> Specific tag OR `.idk{color: blue;}` --> All tags which include idk ka class.

- For specific child tag:- `parenttag childtag {}`

- To give for specific id:- `#(idname) {}`

- To give for a specific tag from the class, while that classs is having other tags too, but others wont change:-

```CSS
p[class="damn"] {color:blueviolet;
padding: 10px;}
```

# Color

1. You can control the color by adjusting the shade, also can control the opacity by clicking the box of that color.
2. Must try rgb tag inside color, red-green-blue

# Background

Can change

## a) **background color**:-

` background color:red;`
To put color only on specific text then use **"span"** tag.

## b) **background img**:-

` background-image:url("abc.jpg")`

## c) **background repeat**:-

Very usefull to repeat certain img/color in given axis or randomly or to stop the repeation

## d) **background position**:-

Can take the img to any direction.

# Fonts

## a) **Font-family**:-

Used to change the fonts into different types. Can also change the font by finding it from **"google fonts"** and pasting the link ref of it
above style tag.

## b) **Font-style**:-

Changes the style like italic,etc.

## c) **Font-size**

## d) **Font-weight**:-

Can change the darkness like bold,normal,light,etc.

# Texts

## a) **text color**:-

`color{}`

## b) **text align**:-

_left, center, right, justify_
(texts is written from left and it ends at right, it covers the whole line).

## c) **text-decoration** :-

_overline, line through, underline, underline overline._

## d) **text-transform** :-

_capitalize, uppercase, lowercase_

## e) **text-indentation**

## f) **letter-spacing**

## g) **word-spacing**

## h) **text-shadow**:-

` text-shadow: h-shadow v-shadow blur-radius color,`

h-shadow means distance horizontally, v-shadow is distance vertically, blur-radius means part to be blurred, then color.

# Img

To change alignment of img to :-

## a) **Center**:-

u can create style in css

`img{ display:block; margin-left: auto; margin-right: auto;}`

## b) **Left**:-

u can create style in css

` img{ display:block; margin-right: auto;}`

## c) **Right**:-

u can create style in css

` img{ display:block; margin-left: auto;}`

---

# Units in CSS:-

## 2 Types:-

### a) **Absolute units**:-

Its fixed units like cm,m,px,etc.

_1px = 1/92th of 1 inch
1pt = 1/72th of 1 inch
1pc = 12pt_

### b) **Relative units**:-

depends on web page or parent element.

_vw:- 1% width of web page._

_vh:- 1% height of web page._

_vmin:- minimum value among height and width will be used here._

_vmax:- maximum value among height and width will be used here._

# Box Model Styling

- Learn to write texts in box form.

  ## a) **padding**:-

  Gives space before the text starts from the left and right of the boc or the web page. Both side the distance will be same.

  ## b) **Border**:-

  Strong colored border to the text.
  Border itself is a big topic to cover. Basically 6 topics in border which you should consider before using.

  ### 1. **Border-width** :-

  The border-width property specifies the width of the four borders in pixels.

  ### 2. **Border-style** :-

  There are total 11 types of borders which you could give to the table.

  ### 3. **Border-color** :-

  The border-color property is used to set the color of the four borders.

  ### 4. **Border-Shorthand** :-

  Basically width, style & color written in same syntax.

  - EG:-` border: 5px solid red;`

  ### 5. **Border-sides** :-

  Can individually give the tpye of style of border on each side like top, botton, left, right.

  ### 6. **Border-radius** :-

  Can make the border rounder in pixels.

  ## c) **Margin**:-

  Same like padding, just the difference is that the background color wont be seen into margin. Only if the parent tag ka color changes
  then the margin will be filled.

  ## d) **Box-sizing-border box** :-

  Very important element to be used for whole html file. It will add padding & border (width,solid color) without affecting
  the size of box. So if there are 2 boxes then both will be aligned even if one box adds any padding to the texts.

  # Styling Lists

  Here, we modify the bullets using style.

  ## a) **list-style-type**

  ## b) **list-style-position**

  ## c) **list-style-image**

# Some important Selectors

_**Hover,visited,link,float,hidden.**_

**Hover**:- Changes will be made when we move our cursor to it.

**Visited**:- Changes in color or etc will be made once we visit that link.

**Float & overflow hidden**:- Box model se bahar aajate h texts. It wont be seen unless u use overflow hidden. As the text is overflowed out of the box.

# Styling Tables

## Table Border:-

### 2 types:-

#### a) **Separate border**:- Separate blocks.

#### b) **Collapse border**:- Joint blocks.

_Style to change these two types_:-

```CSS
border-collapse: collapse; OR border-collapse: separate;
```

c) **padding**:- To give spacing between the texts in the block of table.
`th,td{padding:15px;}`

d) **border-spacing**:- To give spacing between the tables.

# Specificity

- If there are two or more CSS rules that point to the same element, the selector with the highest specificity value will "win", and its style declaration will be applied to that HTML element.

- Also, the element written most recently will be applied to the txt.

# Controlling inheritance:-

## 1. **Unset**:-

Unset is a CSS value that's the same as "inherit" if a property is inherited or "initial" if a property is not inherited.

## 2. **Initial**:-

The initial value of a CSS property is its default value which differs with websites.

## 3. **Inherit**:-

The inherit keyword specifies that a property should inherit its value from its parent element.

## 4. **Default**:-

Default value of any element. eg:- link ka purple hota h.

## 5. **Important**:-

Important ka specificity is the most.

```css
!important.
```

# Controlling Overflow out of box:-

Overflow of text outside the box happens when the width and height of the box is small compared to text.
To solve this, we use:-
overflow:-

```CSS
 Syntax---> overflow: scroll/auto/hidden/visible;
```

**Difference** in auto and scroll is that the box can be scrolled even after the width is sufficient in case of scroll, but in auto it'll not scroll.

# Controlling img out of box:-

Sytnax to fit img inside the box:-

```CSS
 object-fit: cover/contain/fill.
```

# Payment File Explanation:-

## 1. **Box-sizing-border box** :-

- Very important element to be used for whole html file.
- It will add padding & border (width,solid color) without affecting the size of box.
- So if there are 2 boxes then both will be aligned even if one box adds any padding to the texts.

## 2. **Body**:-

Whatever background is added (Here, whitesmoke) will be affected on the full web page.

## 3. **Importing font**:-

Always write the import code at the beginning of any style.

## 4. Width: 100% :-

This % is according to the web page.

## Practice Q)

Contact_test :-

**body**:-
Background color of web page is the background-color of the body.

**h1**:-
Margin of h1 is the distanace of h1 text from the table. It also changes the size of the box, as the distance is getting increased which means border will move far along with the box.

**div**:-
background-color of the box in which text is written.
border is for the white box to get green color at the corners.

# Debugging in CSS

Right click krne se on any web page, you'll see option to _**"view page source"**_ & _**"Inspect"**_.

1.  **View page source**:- Can view full code written to make that particular web page.
2.  **Inspect**:- Just explore it yourself, kind of same to view page. Computed option bhi explore krna. Debugging is usually done with this, styles waale option se.

> RECOMMENDED:- View the box ke dimensions, the way padding, width, height are applied.

_Difference in view page source & inspect_:- Syntax mai koi error hua then it wont be corrected in view page source on the otherr hand, in inspect the correct code will be displayed.

# Clip path generator:-

- Used to change the size and shape of the image without putting much efforts.
- Search "_**Clip path generator**_" on google then select appropriate shape, copy the url & paste in the CSS.

---

## _Difference in box-sizing.border-box & box-sizing.content-box :-_

```
  width: 160px;
  height: 80px;
  padding: 20px;
  border: 8px solid
```

- **box-sizing: content-box**;

  - { **Total width**: 160px + (2 _ 20px) + (2 _ 8px) = 216px. _Left & right padding and border are added._

  - **Total height**: 80px + (2 _ 20px) + (2 _ 8px) = 136px

  - **Content box width**: 160px

  - **Content box height**: 80px
    }

- **box-sizing: border-box**;

  - **Total width**: 160px Width remains the same and both the padding and border are added into the width itself.

  - **Total height**: 80px

  - **Content box width**: 160px - (2 _ 20px) - (2 _ 8px) = 104px

  - **Content box height**: 80px - (2 _ 20px) - (2 _ 8px) = 24px \_/

# CSS Layers:-

1. z-index :-
   - Used to give the priority number to the overlapping boxes.
   - The eg of box overlap will be in html files.
   - Greater the number of index, more will be the priority, means it'll be at the top.
   - Using "position" is important & necessary with z-index.

# Responsiveness

- Responsive web design makes your web page look good on all devices.
- It varies with the change in the width of the screen.
- We use "**and**" operator to change the layout with respect to the width.
- To use "**or**" operator simple add another ',' after the 'and ()'.

  ```CSS
   @media screen and (max-width:400px), (max-width:1000px); {   } .
   @media , @media screen, etc.
  ```

  > NOTE:- Div is used to write text in a given block. It doesnt use the whole line like p tag. So, div is used for writing text with space in the same line.

- Use **box-sizing: border-box** for viewing the text in box in the same line.

- Solved a problem stmt, check it out:-

  [Responsiveness](https://codepen.io/Vansh-Baghel/pen/eYVOxQN)

  **NOTE**:- Use inspect option and change the width of the page to see the changes.

# Display

> Syntax:- display : (value);

## Types of Values

### 1. **Inline** :-

Displays an element in the same line. (like `<span>`).

- Any height and width properties will have no effect.

### 2. **Block**:-

Displays an element which starts on a new line, and takes up the whole width. It adjusts the box into the column by default.

### 3. **Flex** :-

Displays the boxes in the row adjacent to each other. More better and detailed explanation in flex heading.

### Tags important to use with display tag.

#### 1. **Float**:-

Used to adjust the img or text in any direction.

- None :- The element does not float (will be displayed just where it occurs in the text). This is default.

```CSS
float: left/right/none/inherit;
```

#### 2. **Clear**:-

Used to specify what should happen with the element that is next to a floating element.

```
clear: left/right/none/inherit/both;
```

### 3. **Position** :-

1. **Static**:- It is not affected by the top, bottom, left, and right properties.

- HTML elements are positioned static by default.

2. **Relative**:- top, right, bottom, and left properties of a relatively-positioned element will cause it to be adjusted away from its normal position.

   EG:-

```CSS
{position: relative;
 top:10px;
}
```

3. **Fixed**:- This position of it will remain at the same place on the screen even if we scroll the pg.

4. **Sticky**:-

- A sticky element toggles between relative and fixed.
- If, we give `top,bottom` tags of relative, then it'll act as fixed (it'll not move even if we scroll) .

- Else, using sticky doesnt make any difference.

5. **Absolute**:- This will overlap the boxes and the text.

### Challenge question:- [Position_clear_float_responsiveness](https://codepen.io/Vansh-Baghel/pen/ZErzwoz)

- _**Explanation**_ :-

1. **Url method**:- Copy the link address of img from google so you dont need to place the downloaded file in the folder.

2. **Class** :-

- Here, 2 classes are in one `<div class="box box-1">` , which means ki box will be used as common class if you want any change in 3-4 steps & box-1 will be unique for that particular (basically to change the position it must be unique).
- Also, can use class in img.

3. **p** :-

- We need to use paragraph tag to write the text bcoz we need the text besides the img, if u use div then the text will be visible down to the image.

* If you want to view the text on same line by using _div_, better use `display:inline` for viewing the text besides the img.

- We can add clear, align tags for p to adjust the text for _@media_.

4. **div in css** :-

- _Overflow_ is used to hide the overlapping of texts while changing the width.
- _Widht & height_ are in vw & vh which means % of the web pg.
- _Margin_ is used in shortcut method whose syntax is

```CSS
margin:top right bottom left
```

5. **img in CSS** :-

- Box type around image in added by changing height & width of it.

6. **@media** :-

- _Text_ is aligned to center and its cleared from both the side so that we dont need to adjust the text again & again when the image is left & right.

### Challenge Question:- [Position_sticky](https://codepen.io/Vansh-Baghel/pen/PoQoPNx)

_**Explanation**_ :-

- Used **div** and added class for both a and p tags.
  Adding class in both the tags are important, bcoz the div tag with class will also be changed if we try to change the normal div tag.

* **CSS edits**
  - `.nav1` :-
    - We need to add background color for navigation to this tag, bcoz div tag extends throughout the line.
    - While adding background color to the a tag, it would've been visible in that small particular short block and not the whole line.

# Flexbox

- To start with flexbox, we first need to understand its terminologies.

![Terminolgy](https://miro.medium.com/max/1183/1*ubDrM-3m22gLF_pZ4DCdMw.png)

## Elements

### 1) **display:block/flex**:-

- Difference in both is that block adjusts the boxes into 1 column and flex adjust in 1 row.
- Anyways, we could change the direction of box using different element tag.

### 2) **flex-direction:(value)** :-

- Here are some values which we use with this element.

  a) **row** :- Adjusts the boxes in same row.

  b) **column** :- Adjusts the boxes in same column.

  c) **column-reverse** or **row-reverse** :- Adjusts the boxes in same as column or row, but in reverse order.

### 3. **justify-content:(values)** :-

- Here are some values which we use with this element.

  a) **flex-start**

  b) **flex-end**

  c) **center**

  d) **space-around** :-

  - This tag has same padding space between them ; and the space before and after the box are same.
  - The space between & before-after are different.

  e) **space-between** :- Items will have space between them but not before and after it.

  f) **space-evenly** :-

  - Items will have equal space around them.
  - Here, the space between, before and after all are same.

### 4. **align-items: (values)** :-

- Used to change the position of boxes.

- Some values are:-

  a) **center**

  b) **flex-start** :- Items are positioned at the beginning.

  c) **flex-end** :- Items are positioned at the end.

  d) **stretch** :- Stretches and increases the height of the box w.r.t the web page.

  e) **baseline** :- Items are positioned at the baseline of the container.

### 5. **align-self: (values);**

- Same values like align-items, its just used to move some boxes particularly .

### 6. **flex:wrap;(values)**

- Some values:-
  - a) wrap:- Used to change the width of screen without changing the size of box. The box will appear on new line rather than shrinking.
- There are more values, you can explore them too.

### 7. **align-content**:-

The align-content property modifies the behavior of the flex-wrap property. It is similar to align-items, but instead of aligning flex items, it aligns flex lines.

### 8. **Order** :-

Can change the order of any box individually.

### 9. **flex-basis** :-

Used to give the max width to boxes.

### 10. **flex-grow:(value)** :-

- Here, value is in the form of number, which represents the speed.
- Here, the size of the box will grow at certain speed & resolution when the width of web pg in increased.

### 11. **flex-shrink:(value)** :-

- Same as grow, just the opposite happens.
