# Neumorphism for Harmony OS

# Installation :

Install using npm

```npm i hmos-neumorphism ```

# Note :

Add this css snippet when passing input or button through slot .

```css
button, input{
    width: 100%;
    height: 100%;
    background-color:transparent;
    text-color: black;
}
```

# Import all components at once

```html
<element name='neutheme' src='../../../../../../node_modules/hmos-neumorphism/theme/theme.hml'></element>
<element name='neualert' src='../../../../../../node_modules/hmos-neumorphism/alert/alert.hml'></element>
<element name='neuavatar' src='../../../../../../node_modules/hmos-neumorphism/avatar/avatar.hml'></element>
<element name='neubutton' src='../../../../../../node_modules/hmos-neumorphism/button/button.hml'></element>
<element name='neubuttons' src='../../../../../../node_modules/hmos-neumorphism/buttons/buttons.hml'></element>
<element name='neucard' src='../../../../../../node_modules/hmos-neumorphism/card/card.hml'></element>
<element name='neucheckbox' src='../../../../../../node_modules/hmos-neumorphism/checkbox/checkbox.hml'></element>
<element name='neudropdown' src='../../../../../../node_modules/hmos-neumorphism/dropdown/dropdown.hml'></element>
<element name='neuform' src='../../../../../../node_modules/hmos-neumorphism/form/form.hml'></element>
<element name='neuinput' src='../../../../../../node_modules/hmos-neumorphism/input/input.hml'></element>
<element name='neulabel' src='../../../../../../node_modules/hmos-neumorphism/label/label.hml'></element>
<element name='neunavbar' src='../../../../../../node_modules/hmos-neumorphism/navbar/navbar.hml'></element>
<element name='neupagination' src='../../../../../../node_modules/hmos-neumorphism/pagination/pagination.hml'></element>
<element name='neuprogress' src='../../../../../../node_modules/hmos-neumorphism/progress/progress.hml'></element>
<element name='neuradio' src='../../../../../../node_modules/hmos-neumorphism/radio/radio.hml'></element>
<element name='neuswitcher' src='../../../../../../node_modules/hmos-neumorphism/switcher/switcher.hml'></element>
<element name='neucarousel' src='../../../../../../node_modules/hmos-neumorphism/carousel/carousel.hml'></element>
```

# Theme

<p float="left">
<img src="sample_images/theme1.png" width="" height="">
<img src="sample_images/theme2.png" width="" height="">
<img src="sample_images/theme3.png" width="" height="">
</p>

Import:
```html
<element name='neutheme' src='../../../../../../node_modules/hmos-neumorphism/theme/theme.hml'></element>
```

Usage:
```html

<!--You can choose between following themes:-->

<!--white-->
<!--silver-->
<!--gray-->
<!--black-->
<!--red-->
<!--maroon-->
<!--yellow-->
<!--olive-->
<!--lime-->
<!--green-->
<!--aqua-->
<!--teal-->
<!--blue-->
<!--navy-->
<!--pink-->
<!--purple-->

<neutheme theme="silver" text="black">
</neutheme>
```

# Alert

<img src="sample_images/alert.png" width="" height="">

Import:
```html
<element name='neualert' src='../../../../../../node_modules/hmos-neumorphism/alert/alert.hml'></element>
```

Usage:
```html
<neualert icon="common/icons/heart.png" width="300px" height="60px" border="40px" >
  <text>Alert !</text>
</neualert>
```

# Avatar

<img src="sample_images/avatar.png" width="" height="">

Import:
```html
<element name='neuavatar' src='../../../../../../node_modules/hmos-neumorphism/avatar/avatar.hml'></element>
```

Usage:
```html
<neuavatar icon="common/icons/user.png" width="100px" height="100px" border="50px"></neuavatar>
```

# Button

<img src="sample_images/button.png" width="" height="">

Import:
```html
<element name='neubutton' src='../../../../../../node_modules/hmos-neumorphism/button/button.hml'></element>
```

Usage:
```html
<neubutton icon="common/icons/heart.png" width="250px" height="60px" border="50px" @button-event="buttonClick">
  <text>Button</text>
</neubutton>
```

# Buttons

<img src="sample_images/buttons.png" width="" height="">

Import:
```html
<element name='neubuttons' src='../../../../../../node_modules/hmos-neumorphism/buttons/buttons.hml'></element>
```

Usage:
```html
<neubuttons  width="250px" height="60px" border="50px">
  <button slot="first" onclick="buttonLeftClick">Left</button>
  <button slot="second" onclick="buttonRightClick">Right</button>
</neubuttons>
```

# Card

<img src="sample_images/card.png" width="" height="">

Import:
```html
<element name='neucard' src='../../../../../../node_modules/hmos-neumorphism/card/card.hml'></element>
```

Usage:
```html
<neucard width="300px" height="200px" border="10px" >
  <image src="common/placeholder.png" ></image>
</neucard>
```

# Checkbox

<img src="sample_images/checkbox.png" width="" height="">

Import:
```html
<element name='neucheckbox' src='../../../../../../node_modules/hmos-neumorphism/checkbox/checkbox.hml'></element>
```

Usage:
```html
<neucheckbox color="" width="50px" height="50px" border="50px" checked="true" @check-event="checkboxClick"></neucheckbox>
```

# Dropdown

<img src="sample_images/dropdown.png" width="" height="">

Import:
```html
<element name='neudropdown' src='../../../../../../node_modules/hmos-neumorphism/dropdown/dropdown.hml'></element>
```

Usage:
```html
<neudropdown width="200px" height="50px" border="10px" @change-event="dropdownSelect">
  <select @change="dropdownSelect">
    <option value="Item 1">Item 1</option>
    <option value="Item 2">Item 2</option>
    <option value="Item 3">Item 3</option>
    <option value="Item 4">Item 4</option>
    <option value="Item 5" selected="true">Item 5</option>
  </select>
</neudropdown>
```

# Form

<img src="sample_images/form.png" width="" height="">

Import:
```html
<element name='neuform' src='../../../../../../node_modules/hmos-neumorphism/form/form.hml'></element>
```

Usage:
```html
<neuform width="350px" height="300px" border="20px" @submit-event="buttonClick" @reset-event="buttonClick">
 <neuinput icon="common/icons/user.png" type="email" maxlength="20" placeholder="Email" border="30px"></neuinput>
 <neuinput icon="" type="password" maxlength="20" placeholder="Password" border="20px"></neuinput>
 <div>
  <neubutton icon="" width="150px" border="20px">
   <input type='submit' style="border-radius:20px;">Submit</input>
  </neubutton>
  <neubutton icon="" width="150px" border="20px">
   <input type='reset' style="border-radius:20px;">Reset</input>
  </neubutton>
 </div>
</neuform>
```

# Input

<img src="sample_images/input.png" width="" height="">

Import:
```html
<element name='neuinput' src='../../../../../../node_modules/hmos-neumorphism/input/input.hml'></element>
```

Usage:
```html
<neuinput icon="common/icons/user.png" type="text" maxlength="20" placeholder="Input" width="300px" height="50px" border="50px" ></neuinput>
```

# Label

<img src="sample_images/label.png" width="" height="">

Import:
```html
<element name='neulabel' src='../../../../../../node_modules/hmos-neumorphism/label/label.hml'></element>
```

Usage:
```html
<neulabel text="Label" icon="common/icons/heart.png" width="200px" height="50px" border="50px" ></neulabel>
```

# Navbar

<img src="sample_images/navbar.png" width="" height="">

Import:
```html
<element name='neunavbar' src='../../../../../../node_modules/hmos-neumorphism/navbar/navbar.hml'></element>
```

Usage:
```html
<neunavbar  width="300px" height="50px" border="50px" @right-event="buttonClick" @middle-event="buttonClick" @left-event="buttonClick">
  <image slot="first" src="common/icons/recent.png" style="width:20px; height: 20px;" ></image>
  <image slot="second" src="common/icons/home.png" style="width:20px; height: 20px;" ></image>
  <image slot="third" src="common/icons/return.png" style="width:20px; height: 20px;" ></image>
</neunavbar>
```

# Pagination

<img src="sample_images/pagination.png" width="" height="">

Import:
```html
<element name='neupagination' src='../../../../../../node_modules/hmos-neumorphism/pagination/pagination.hml'></element>
```

Usage:
```html
<neupagination color="" width="300px" height="50px" border="50px"  @previous-event="previousEvent" @next-event="nextEvent">
  <button>1</button>
  <button>2</button>
  <button>3</button>
  <button>4</button>
  <button>5</button>
</neupagination>
```

# Progress

<img src="sample_images/progress.png" width="" height="">

Import:
```html
<element name='neuprogress' src='../../../../../../node_modules/hmos-neumorphism/progress/progress.hml'></element>
```

Usage:
```html
<neuprogress progress="80%" width="300px" color="" height="20px" border="50px"></neuprogress>
```

# Radio

<img src="sample_images/radio.png" width="" height="">

Import:
```html
<element name='neuradio' src='../../../../../../node_modules/hmos-neumorphism/radio/radio.hml'></element>
```

Usage:
```html
<neuradio width="50px" color="" height="50px" border="50px" checked="" @check-event="radioClick"></neuradio>
```

# Switcher

<img src="sample_images/switcher.png" width="" height="">

Import:
```html
<element name='neuswitcher' src='../../../../../../node_modules/hmos-neumorphism/switcher/switcher.hml'></element>
```

Usage:
```html
<neuswitcher width="60px" color="" height="30px" border="50px" toggle="off" @toggle-event="toggleClick"></neuswitcher>
```

# Carousel

<img src="sample_images/carousel.png" width="" height="">

Import:
```html
<element name='neucarousel' src='../../../../../../node_modules/hmos-neumorphism/carousel/carousel.hml'></element>
```

Usage:
```html
<neucarousel width="300px" height="200px" color="black" border="10px" index="0" indicator="true" loop="true">
            <image src="common/placeholder.png" ></image>
            <image src="common/placeholder.png" ></image>
            <image src="common/placeholder.png" ></image>
        </neucarousel>
```

# Reference:

<a href="https://neumorphism.io/">neumorphism.io</a>

<a href="https://ismail9k.github.io/neomorphism/">ismail9k.github.io/neomorphism</a>
