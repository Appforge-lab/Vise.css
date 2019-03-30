## Approach

Vise is not the usual framework, it's not based only on making CSS styling a faster process but also forged with some notions in mind:

- **Encaplsulation**

  Vise is self-enclosed, it doesn't get affected by previously loaded frameworks on the same HTML document. Thus it can be used alongside any other framework (Bootstrap, Foundation, Bluma, etc).

  Any element enclosed within Vise's opening and closing tags drops any previous alternation and gets Vise's defaults.

  Any Vise class is only usable within Vise's enclosure and affects only it's child elements, leaving outer elements untouched.

- **Self-reliance**

  Packed with the basic features, Vise is functional out-of-the-box. With styled HTML elements, helper classes and a smart grid system, Vise is a complete framework that can build simple and complex web contents.

- **Minimalism**

  Vise is meant to be minimal while offering the basic features to build a consistent user experience. With around 30kb of size, Vise is one of the most lightweight frameworks. Based on a simple naming convention and a powerful grid system, it forms a reliable starting point for your project.

# Vise with Bootstrap

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

# Class Assignement Convention

Vise uses a unique class assignement convention with less hyphens, dashes and a style close to the default CSS naming system. The assignement convention is based on the colon character ":" which is introduced exclusively in Vise framework. The latter makes it effortless to distinguish between the opcode and the operand in a class assignment.

```html
<div class="vise">	
    <div class="fill:blue padding:2">
    <div class="fill:black color-text:orange padding-sides:2">
</div>	
```

[Live demo](http://cssdeck.com/labs/fptegaf0)
