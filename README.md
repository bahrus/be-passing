# be-passing [TODO]

*be-linking* supports an option to pass a value around in a downward direction:


```html
<host-element>
    #shadow
        <input type=number be-linked='
            On input event of $0 
            pass value property as number 
            to slide index property 
            of slide show id 
            within root node.
        '>
        ...
        <my-carousel id=slide-show></my-carousel>
</host-element>
```

*be-passing* supports this scenario with more compact notation:

```html
<host-element>
    #shadow
        <input type=number be-passing='of value to #slide-show on input.'>
        ...
        <my-carousel id=slide-show></my-carousel>
</host-element>
```

```html
<host-element>
    #shadow
        <input type=number be-passing='of value to my-carousel on input.'>
        ...
        <my-carousel></my-carousel>
</host-element>
```
