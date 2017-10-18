<h1 align="center">
  <br>
  <a href=""><img src="logo.png" alt="Pretty checkbox" width="100"></a>
  <br> <br> pretty-checkbox.css <br>
</h1>

<h4 align="center">A pure css library to beautify checkbox and radio buttons.</h4>

<p align="center">
 <a href="#">
    <img src="https://img.shields.io/github/release/lokesh-coder/pretty-checkbox.svg?style=flat-square&colorA=8033b0&colorB=75b7dd" alt="Github Release">
  </a>
   <a href="#">
    <img src="https://img.shields.io/npm/l/pretty-checkbox.svg?style=flat-square&colorA=8033b0&colorB=75b7dd" alt="Licence">
  </a>
   <a href="#">
    <img src="https://img.shields.io/github/size/lokesh-coder/pretty-checkbox/src/pretty.min.css.svg?style=flat-square&colorA=8033b0&colorB=75b7dd" alt="Size">
  </a>
</p>
<br>

<div class="highlight highlight-source-shell">
<pre>
<div align="center"><strong >Demo and documentation</strong></div>
<div align="center"><a align="center" href="https://lokesh-coder.github.io/pretty-checkbox/">https://lokesh-coder.github.io/pretty-checkbox/</a></div>
</pre>
</div>

### Features
* Basic
  - **Shapes** - *Square*, *Curve*, *Round* 
  - **Variants** - *Default*, *Fill*, *Thick*
  - **Colors** - *Primary*, *Success*, *Info*, *Warning*, *Danger* 
  - **Color types** - *Solid*, *Outline*
  - **Animations** - *Smooth*, *Tada*, *Jelly*, *Rotate*
 * Switch - iOS style - *Outline*, *Fill*, *Slim*
 * Responsive
 * No Javascript
 * Custom Font Icons
 * Svg Icons
 * Image 
 * Toggle
 * Lock
 * State - *Focus*, *Hover*, *Inderterminate*
 * Supports frameworks - *Bootstrap*, *Foundation*, *Sematic UI*, *Bulma*, ...
 * Customize nearly everything with SCSS
 * Print friendly
 * and more... ( *I am kidding, thats all!* )

### Installation
- **From CLI**

Install the library from [`npm`](https://www.npmjs.com/package/pretty-checkbox) or [`yarn`](https://yarnpkg.com/en/package/pretty-checkbox) package manager

```sh
> npm install pretty-checkbox // or
> yarn add pretty-checkbox
```
Add `pretty-checkbox.min.css` in your html

<br>

- **From CDN** ( [Jsdelivr ](https://www.jsdelivr.com/package/npm/pretty-checkbox) )
```html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/pretty-checkbox@3/dist/pretty-checkbox.min.css"/>
```

<br>

- **Manual download** ( [Github](https://github.com/lokesh-coder/pretty-checkbox/archive/master.zip) )

Download the source from github
```html
<link rel="stylesheet" href="../<PATH>/pretty-checkbox/dist/pretty-checkbox.min.css"/>
```
`<PATH>` is where the library is downloaded.

<br>

**SCSS**

You can also import `pretty-checkbox.scss` in your main scss file.
```scss
@import '~pretty-checkbox/src/pretty.scss';
```

Please refer the document for SCSS settings.


### Usage


Pretty checkbox comes with many styles,

| Class name  | Description              |
| :---------- | :----------------------- |
| `--default` | Basic style              |
| `--switch`  | iOS like toggle style    |
| `--icon`    | Custom font icons        |
| `--svg`     | Custom SVG files, markup |
| `--image`   | Tiny images              |

And three shapes `--round` `--curve` `--square` (default)


#### Basic checkbox,

```html
<div class="pretty --default">
	<input type="checkbox">
	<div class="state">
		<label>Check me</label>
	</div>
</div>
```

Basic checkbox has three variants `--fill` `--thick` `--outline` (default)

You can combine them.

```html
  <div class="pretty --default --curve --fill">
      <input type="checkbox" />
      <div class="state">
          <label>Fill</label>
      </div>
  </div>
```

<div align="center"><strong >---</strong></div>

#### Switch checkbox,

Switch has three variants `--outline` `--fill` `--slim`

```html
<div class="pretty --switch --fill">
    <input type="checkbox" />
    <div class="state">
        <label>On</label>
    </div>
</div>
```

<div align="center"><strong >---</strong></div>

#### Custom Font icons,

```html
<div class="pretty --icon">
	<input type="checkbox">
	<div class="state">
    	<i class="icon fa fa-check"></i>
		<label>Check me</label>
	</div>
</div>
```

<blockquote>
    <sub>
    	<strong>Note</strong>: class `icon` should be added along with icon class names
    </sub>
</blockquote>

<blockquote>
    <sub>
    	<strong>Note</strong>: For icons to work, you need to add appropriate font icons library. In above example , we used font awesome icon. So, FontAwesome should be included separately. 
    </sub>
</blockquote>

<p> Checkout the documentation for tested font icon libraries.</p>

<div align="center"><strong >---</strong></div>

#### SVG

```html
<div class="pretty --svg">
	<input type="checkbox">
	<div class="state">
    	<img class="svg" src="file.svg">
		<label>Check me</label>
	</div>
</div>
```

Support, SVG file in img tag, svg markup (`<svg> ... </svg>`)

<blockquote>
    <sub>
    	<strong>Note</strong>: class `svg` to be added in img tag or svg tag.
    </sub>
</blockquote>

Checkout the documentation for different formats and tested svg libraries.

<div align="center"><strong >---</strong></div>

#### Image

```html
  <div class="pretty --image">
      <input type="checkbox" />
      <div class="state">
          <img class="image" src="/check.png">
          <label>Block</label>
      </div>
  </div>
```

Supports any type of valid image format.

<blockquote>
    <sub>
    	<strong>Note</strong>: class `image` to be added in img tag.
    </sub>
</blockquote>

Checkout the documentation for different formats and tested svg libraries.

<div align="center"><strong >---</strong></div>

#### Colors

There are five solid colors `--primary` `--success` `--warning` `--info` `--danger`

And five outline colors  `--primary-o` `--success-o` `--warning-o` `--info-o` `--danger-o`

```html
  <div class="pretty --default --curve --thick">
      <input type="checkbox" />
      <div class="state --warning">
          <label>Warning</label>
      </div>
  </div>
```
<blockquote>
    <sub>
    	<strong>Note</strong>: Color class must be added in state class. Solid colors and Ouline colors have distinct role in font icons and toggle feature.
    </sub>
</blockquote>

Checkout the documentation for complete demo of color combinations with above styles.

### More

There are more features like  ***Radio buttons*** , ***Toggle*** , ***States*** , ***Animations*** , ***Border less*** , ***Lock*** , ***Scale***, ***SCSS Settings***. 

Please refer the documentation to know about them.


### Browser support
`IE >= 10`   `Firefox >= 3.6`   `Chrome >= 14`   `Safari >= 6`   `Opera >= 11.6`

### Font Icon libraries
* [Font awesome](http://fontawesome.io/icons/)
* [Bootstrap Glyphicons](https://getbootstrap.com/docs/3.3/components/#glyphicons)
* [Material icon ( MDI )](https://materialdesignicons.com/)
* [Material icon ( ZMDI )](http://zavoloklom.github.io/material-design-iconic-font/icons.html)
* [Ion icons](http://ionicons.com/)
* [Typicons](http://www.typicons.com/)
* [Material icon ( Google )](https://material.io/icons)
* Others not tested, but will work ( 99% ).


### SVG
* [UIKit](https://getuikit.com/docs/icon)
* [Feathers](https://feathericons.com/)
* Others

### Inspiration
- [awesome-bootstrap-checkbox](https://github.com/flatlogic/awesome-bootstrap-checkbox) - Idea
- [Animista](http://animista.net) - Animations

### Contributions
Thanks to all those good people who spend their valuable time and helped to improve this library. Any Contributions are welcome!

### Licence
This project is licensed under the MIT License


<div align="center"><sub>❤</sub></div> 
