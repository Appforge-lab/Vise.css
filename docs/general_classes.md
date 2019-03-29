# GENERAL CLASSES

Vise comes with built-in general purpose classes intended to make things faster. They can be used anywhere within Vise's scope and they are: **fill**, **color**, **style**, **opacity**, **radius**, **shadow/outline**, **padding**, **width/height**, **align**, **adapt**, **reset**.



## FILL / COLOR

Used to fill an element's background with a color from the palette below. For text coloring, **color** can be used.

```html
<div class="vise">
  <div class="fill:blue color:aqua">Text</div>
  <div class="fill:red color:white">Text</div>
  <div class="fill:green color:black">Text</div>
</div>
```

[Live demo](http://cssdeck.com/labs/kbrc3xmv)

#### COLOR PALETTE

Vise is served with a modern looking color palette from [clrs.cc](https://clrs.cc/) that can be attributed to **color** class.

<img src="http://appforgelab.com/vise/color-palette.svg"/>


## STYLE

Used to style an element, **style** applies a background color and a text color from the style palette below to an element. It accepts the following values: *basic*, *prime*, *aux*, *win*, *pass*, *warn*, *info*, *alert* .

```html
<div class="vise">
  <div class="style:prime">Prime</div>
  <div class="style:warn">Warn</div>
  <div class="style:info">Info</div>
</div>
```

[Live demo](http://cssdeck.com/labs/v3htkdrv)

#### **STYLE PALETTE**

A background and text color palette to express main web events. 

<img src="http://appforgelab.com/vise/style.svg"/>



## OPACITY

Used to set an element's opacity, it accepts up to 13 values  [*1-12*, *max*]

```html
<div class="vise">
  <div></div>
  <div class="opacity:5"></div>
</div>
```

[Live demo](http://cssdeck.com/labs/zaeleyhacg)



## RADIUS

Used to set an element's corners radius, it accepts up to 13 values  [*1-12*, *max*]

```html
<div class="vise">
  <div></div>
  <div class="radius:5"></div>
</div>
```

[Live demo](http://cssdeck.com/labs/mrcm9fkn)



## SHADOW / OUTLINE

**Shadow** is used to create a light shadow for an element. **Outline** is used to apply a contouring outline on an element. Both **Shadow** & **Outline** don't accept values for the current release.

```html
<div class="vise">
  <div class="outline">Text</div>
  <div class="shadow">Text</div>
</div>
```

[Live demo](http://cssdeck.com/labs/z34mwsq0ef)



## PADDING

Used to generate space around an element's content, **padding** accepts up to *13* distinct values ranging from *1* to *12* and *max*. It also comes with the following variants: **padding-sides**, **padding-ends**.

```html
<div class="vise">
  <div class="padding">Text</div>
  <div class="padding:5">Text</div>
  <div class="padding:max">Text</div>
</div>
```

[Live demo](http://cssdeck.com/labs/jhnsgjre)

#### VARIANTS

- **padding-sides** appends a space to left and right of element's content.

  ```html
  <div class="vise">
    <div class="padding-sides">Text</div>
    <div class="padding-sides:5">Text</div>
    <div class="padding-sides:max">Text</div>
  </div>
  ```

  [Live demo](http://cssdeck.com/labs/lrl2ejld)

- **padding-ends** appends a space to the top and bottom of element's content.

  ```html
  <div class="vise">
    <div class="padding-ends">Text</div>
    <div class="padding-ends:5">Text</div>
    <div class="padding-ends:max">Text</div>
  </div>
  ```

  [Live demo](http://cssdeck.com/labs/lrl2ejld)




## WIDTH / HEIGHT

Used to set an element's width/height and similarly to **padding**, they both accept up to *14* values [*1-12*, *min*/*max*] although distinctively, they adopt <u>fixed sizes</u> and <u>common percentages</u>. 

```html
<div class="vise">
  <div class="width:5">Text</div>	
  <div class="width:max">Text</div>
  <div class="height:5">Text</div>
  <div class="height:max">Text</div>
</div>
```

[Live demo](http://cssdeck.com/labs/v02wajqp)

- **Fixed sizes:** *16*, *24*, *32*, *48*, *64*, *80*, *96*, *128*, *256*, *640*, *768*, *960*, *1024*, *1280*, *1440*

  ```html
  <div class="vise">
    <div class="width:64">Text</div>
    <div class="width:128">Text</div>
    <div class="height:64">Text</div>
    <div class="height:128">Text</div>
  </div>
  ```

  [Live demo](http://cssdeck.com/labs/8fqtmqc9)

- **Common percentages:** *fifth*, *third*, half

  ```html
  <div class="vise">
    <div class="width:fifth">Text</div>
    <div class="width:third">Text</div>
    <div class="height:fifth">Text</div>
    <div class="height:third">Text</div>
  </div>
  ```

  [Live demo](http://cssdeck.com/labs/vcnxzwok)

**Width** has **width-max** variant intended to allow the shrinkage of an element, thus employed for a responsive behavior. It accepts the following values: *640*, *768*, *960*, *1024*, *1280*, *1440*.

```html
<div class="vise">
  <div class="width-max:1280">Text</div>
</div>
```

[Live demo](http://cssdeck.com/labs/bqh0yabu)



## ALIGN

Used to align elements within a container, **align** is specific to **row**/**col** grids, although **align-text** is a variant of it that can be used anywhere within Vise's scope for a horizontal alignment of elements.

```html
<div class="vise">
  <div class="align-text:center">Text</div>
</div>
```

[Live demo](http://cssdeck.com/labs/rhjeamtz)



## ADAPT

**Adapt** is a general purpose class used to adapt elements to a distinct screen width to ensure responsive ability. It considers *3* screen sizes: **adapt-small**, **adapt-medium** and **adapt-large**. In the general use case, **adapt** accepts *3* values: *stretch*, *show* and *hide* but when used with **row**/**col** it permits the use of *2* more values: *switch* and [*1-12*, *min*/*max*].

```html
<div class="vise">
  <div class="adapt-small:hide"></div>
  <div class="adapt-medium:hide"></div>
  <input type="text" name="" class="width:third adapt-medium:stretch">
</div>
```

[Live demo](http://cssdeck.com/labs/hq4s6bik)

**N.b.** 

- **Adapt** with no screen size specification has no effect.

- *Switch* and [*1-12*, *min*/*max*] are covered in **row** and **col** sections. 



## SHOW / HIDE

Shows or hides an element.

```html
<div class="vise">
  <div class="fill:blue hide">Text</div>
  <div class="fill:blue show">Text</div>
</div>
```

[Live demo](http://cssdeck.com/labs/pe2kv6lh)



## RESET

Removes any styling applied to an element, **reset** changes elements attributes to Vise's defaults.

```html
<div class="vise">	
  <div class="reset"></div>
</div>	
```

[Live demo](http://cssdeck.com/labs/6lr5c0nr)
