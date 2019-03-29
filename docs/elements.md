# ELEMENTS

Elements enclosed within Vise gets styled according to Vise's style-line. It is planned to cover most of the HTML elements in future releases, however for now only the following elements are styled: **h1** to **h6**, **b**, **strong**, **small**, **table**, **a**, **select**, **textarea**, **lists**, **radio**/**checkbox** and **inputs** of type: *text*, *email*, *number*, *search*, *tel*, *url*, *password*, *submit*, *reset*, *button*.


- Typography: **h1** to **h6**, **b**, **strong**, **small**, **a**

  [Live demo](http://cssdeck.com/labs/8k0gzi7f)

- Lists: ul, li, ol

  [Live demo](http://cssdeck.com/labs/nozhcahn)

- **Inputs** of type: *text*, *email*, *number*, *search*, *tel*, *url*, **select**, **textarea**,.

  [Live demo](http://cssdeck.com/labs/9rggntje)

- Table

  [Live demo](http://cssdeck.com/labs/actgq3my)



## BUTTON

As an essential part of the user experience and by default, any input of type *button* within Vise's enclosure gets the *default* button style demonstrated below. To express common web events, 10 more styles are provided and can be applied to **button** class. Also, a special **hover** class is available with the purpose of adapting button's visibility on low/high lightness backgrounds.

```html
<div class="vise">  
    <input type="button" value="button">
</div>  
```

[Live demo](http://cssdeck.com/labs/buhanvcn)

### BUTTON STYLES

Vise comes packed with the following button styles: light, dark, *basic*, *prime*, *aux*, *win*, *pass*, *warn*, *info*, *alert*. For an inverted style it is possible to use the followings: light-i, dark-i, *basic*-i, *prime*-i, *aux-i*, *win-*i, *pass-i*, *warn-i*, *info*-i, *alert*-i.

```html
<div class="vise">
    <input type="button" class="button:dark">
    <input type="button" class="button:light">
    <input type="button" class="button:basic">
    <input type="button" class="button:prime">
    <input type="button" class="button:aux">
    <input type="button" class="button:win">
    <input type="button" class="button:pass">
    <input type="button" class="button:warn">
    <input type="button" class="button:info">
    <input type="button" class="button:dark-i">
    <input type="button" class="button:light-i">
    <input type="button" class="button:basic-i">
    <input type="button" class="button:prime-i">
    <input type="button" class="button:aux-i">
    <input type="button" class="button:win-i">
    <input type="button" class="button:pass-i">
    <input type="button" class="button:warn-i">
    <input type="button" class="button:info-i"> 
</div>  
```

[Live demo](http://cssdeck.com/labs/obllgv3i)

### HOVER

In certain scenarios, when hovering a button placed on lighter/darker background, the latter may become difficult to notice and for better visibility we provided a **hover** class that changes the hover color to white/black making hover effect more outstanding. **Hover** accepts 2 values: *light* and *dark*.

```html
<div class="vise">  
    <input type="button" value="button" class="button:prime"> 
    <input type="button" value="button" class="button:prime hover:light">
</div>
```

[Live demo](http://cssdeck.com/labs/us7hwlym)



## RADIO / CHECKBOX

Differently to other inputs, **radio** and **checkbox** are not styled on their own, instead they get styled when wrapped inside **box-radio**/**box-checkbox** containers which are variants of **box** (covered below).

```html
<div class="vise">
    <div class="box-checkbox">
        <input type="checkbox">
        <label></label>
    </div>
    <div class="box-checkbox">
        <input type="checkbox">
        <label></label>
    </div>
    <div class="box-radio">
        <input type="radio">
        <label></label>
    </div>  
    <div class="box-radio">
        <input type="radio">
        <label></label>
    </div>
</div>
```

[Live demo](http://cssdeck.com/labs/sckh7hq0)
