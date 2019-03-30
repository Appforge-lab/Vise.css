# VISE

An essential feature of Vise is the ability to be used alongside other frameworks. In the following example we loaded Bootstrap and Vise to create two separate grid systems.

```html
<div class="container">
    <div class="row">
        <div></div>
        <div></div>
    </div>
</div>
<div class="vise">
    <div class="row">
        <div></div> 
        <div></div>
        <div ></div>      
    </div>
</div>
```

[Live demo](http://cssdeck.com/labs/kmeopejy)

# ASSIGNEMENT CONVENTION

Vise uses a unique class assignement convention with less hyphens, dashes and a style close to the default CSS naming system. The assignement convention is based on the colon character ":" which is introduced exclusively in Vise framework. The latter makes it effortless to distinguish between the opcode and the operand in a class assignment.

```html
<div class="vise">	
    <div class="fill:blue padding:2">
    <div class="fill:black color-text:orange padding-sides:2">
</div>	
```

[Live demo](http://cssdeck.com/labs/fptegaf0)
