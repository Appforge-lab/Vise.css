# GRID

Based on flexbox, Vise's grid is designed to build flexible layouts and mobile-first pages. It proposes a row/column structure to horizontally and vertically arrange enclosed elements while offering up to *13* predefined child element sizes. 

The grid system consists of rows and columns with each of them being an independent grid meant to act containers for elements we intend to arrange.

```html
<div class="Vise">
    <div class="row">
        <div></div>
        <div></div>
    </div>
    <div class="col">
        <div></div>
        <div></div>
    </div>
</div>
```

[Live demo](http://cssdeck.com/labs/salyee3a)

Besides the **row**/**col**, a general purpose **box** container is provided to act as a wrapper around elements and to isolate child elements from their **row**/**col** parents.



## REGULAR SIZING

Grid's regular sizing system is an approach proposed to provide a way to size elements enclosed within **row**/**col** proportionally to its container's size. It allows up to *13* distinct sizes [*1-12*, *max*] applied to **row**/**col**/**box**.

```html
<div class="Vise">
    <div class="row">
        <div class="row:5"></div>
        <div class="col:7"></div>
        <div class="box:3"></div>
    </div>	
</div>
```

[Live demo](http://cssdeck.com/labs/tw0tbvpi)



## ROW

Row is a grid that directs child elements to the x-axis and presents elements horizontally one after another separated with a gap if specified.

```html
<div class="Vise">
    <div class="row">
        <div></div>		
        <div></div>	
        <div></div>	
    </div>	
</div>
```

[Live demo](http://cssdeck.com/labs/ec1j9rle)

#### ESSENTIALS

- **Row** should be the first class specified in a <u>div</u> clause with no preceding characters.

- **Row** will take-up the full width of its parent container due to the *100%* default width parameter.

- **Row** has a minimum height of *1.4em*.

  ```html
  <div class="Vise">
      <div class="row"></div>	
  </div>
  ```

  [Live demo](http://cssdeck.com/labs/ii1qvlon2l)

- **Row** is intended to work with general purpose classes, **gap**, **regulate** and **align**.

  ```html
  <div class="Vise">
      <div class="row padding:2 gap:2 color:silver width:5-10 style-shape:oval">
          <div></div>
          <div></div>	
          <div></div>	
      </div>	
  </div>
  ```

  [Live demo](http://cssdeck.com/labs/7vcbkmkf)

- **Row** allows *13* possible unique child elements sizes [*1*-*12*, *max*]

  ```html
  <div class="Vise">
      <div class="row">
          <div class="row:5"></div>
          <div class="row:8"></div>
          <div class="row"></div>
      </div>	
  </div>
  ```

  [Live demo](http://cssdeck.com/labs/wjfi8h64)

#### GAP

Used to generate space between child elements, **gap** is exclusive to **row**/**col** and can't be used anywhere else. It accepts *14* values  [*1*-*12*, *min/max*].

```html
<div class="Vise">
    <div class="row gap">
        <div></div>
        <div></div>
        <div></div>
    </div>
    <div class="row gap:5">
        <div></div>
        <div></div>
        <div></div>
    </div>
    <div class="row gap:max">
        <div></div>
        <div></div>
        <div></div>
    </div>
</div>
```

[Live demo](http://cssdeck.com/labs/azpoxpac)

#### REGULATE

Regulate is a class exclusive to **row**/**col** grids which regulates child elements sizes and allows grid's regular sizing system to be used on each child element or proportionally size elements in case of no explicit sizing specification.

```html
<div class="Vise">
	<div class="row regulate:off">	
		<div></div>		
		<div></div>	
		<div></div>	
	</div>
	<div class="row regulate">	
		<div></div>		
		<div></div>	
		<div></div>	
	</div>
</div>
```

[Live demo](http://cssdeck.com/labs/vvypdha0)

**N.b.**

- Regulate is **active** by default on rows.
- The use of the sizing system on child elements automatically enables **regulate** even if it was explicitly disabled.

#### **ADAPT (Switch)**

> Adapt is a general purpose class used to adapt elements to a distinct screen width to ensure responsive facility. In the general use case, adapt accepts three values: stretch, hide and [*1-12, max*], but when used with rows it permits the use of one more value and that is switch.

**Switch** is a manner to inform one row to change behavior when a particular screen width is met. It forces a **row** to shift to a **col** and direct elements toward the y-axis while keeping the gap.

```html
<div class="Vise">
	<div class="row adapt-medium:switch">
		<div></div>
		<div></div>
		<div></div>
	</div>	
</div>
```

[Live demo](http://cssdeck.com/labs/agmsekaw)

#### ALIGN

Used to align elements within a container, **align** is specific to **row**/**col**. It can align elements horizontally and vertically within a container and accepts the following values : *left*, *center*, *right*, *top*, *middle*, *left*. Additionally it accepts more complex values composed from simple ones: *left-middle*, *center-top*, etc provided to simplify alignment definition.

```html
<div class="Vise">
	<div class="row align:center align:middle">
		<div></div>
	</div>
	<div class="row align:left align:bottom">
		<div></div>
	</div>
	<div class="row align:top-right">
		<div></div>
	</div>
</div>
```

[Live demo](http://cssdeck.com/labs/twgpmcoq)

**N.b.**

- Using **align** will turn off **regulate** if active.
- For a successful vertical alignment, container's height should be superior to element's hight.



## COL

Contrary to **row**, **col** is a grid that directs child content to the <u>y-axis</u> and presents elements <u>vertically</u> one <u>under</u> another separated with a gap if specified.

```html
<div class="Vise">
	<div class="col">	
		<div></div>		
		<div></div>	
		<div></div>	
	</div>	
</div>
```

[Live demo](http://cssdeck.com/labs/bkghxhny)

#### ESSENTIALS

**Col** is similar in most ways to row except for arrangement direction, thus it shares much of the behavior associated with rows:

- **Col** should be the first class specified in a <u>div</u> clause with no preceding characters.
- **Col** will take-up the full width of its parent container due to the *100%* default width parameter.
- **Col** has a minimum height of *1.4em*.
- **Col** is intended to work with general purpose classes, **gap**, **regulate** and **align**.
- **Col** allows *13* possible unique child elements sizes [*1*-*12*, *max*]

#### REGULATE

**Regulate** on **col** has the same behavior as on **row** except that it is **inactive** by default and needs to be explicitly specified.

```html
<div class="Vise">
	<div class="col">	
		<div></div>		
		<div></div>	
		<div></div>	
	</div>
	<div class="col regulate">	
		<div></div>		
		<div></div>	
		<div></div>	
	</div>	
</div>
```

[Live demo](http://cssdeck.com/labs/ujrlrxah)



## BOX

**Box** is a wrapper around elements and is primarily used to isolate child content of **row**/**col** grids, enable the regular sizing system to sizing-incapable elements and regrouping.

```html
<div class="Vise">
	<div class="row">
		<input type="button" class="box:2" value="button">	
		<div class="box:7">
			<div></div>
			<div></div>	
		</div>	
		</div>	
</div>
```

[Live demo](http://cssdeck.com/labs/vuij8oyd)

#### ESSENTIALS

As seen with **col**/**row**, **box** also shares the same essentials with grids but have a different behavior with no alternation of display direction of contained elements.

- **Box** should be the first class specified in a <u>div</u> clause with no preceding characters.
- **Box** will take-up the full width of its parent container due to the *100%* default width parameter.
- **Box** has a minimum height of *1.4em*.
- **Box** is intended to work with general purpose classes.
- **Box** allows *13* possible unique child elements sizes [*1*-*12*, *max*]



# VOID

Void is a vertical spacer intended to separate elements. It can be used anywhere within Vise's enclosure and inside row/col grids. It accepts up to 14 values  [*1*-*12*, *min/max*].

```html
<div class="Vise">
    <div></div>
    <div class="void:5"></div>
    <div></div>
    <div class="void:max"></div>		
    <div></div>
</div>
```

[Live demo](http://cssdeck.com/labs/wtspinkm)
