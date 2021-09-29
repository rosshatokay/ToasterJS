# ToasterJS
Create toaster notifications with a few lines of code.

For quick examples and demos, head to [Live site](https://rosshatokay.github.io/ToasterJS/).

## Installation

You can install ToasterJS from the repository:

```html
<!-- Remember to include jQuery :) -->
<script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.0.0/jquery.min.js"></script>

<!-- ToasterJS -->
<script src="https://raw.githubusercontent.com/rosshatokay/toasterjs/main/src/toaster.js"></script>
<link rel="stylesheet" href="https://raw.githubusercontent.com/rosshatokay/toasterjs/main/src/toaster.css" />
```

## Documentation

You can find the full documentation page [here](https://rosshatokay.github.io/ToasterJS/)

## Getting started

To generate a basic toast, i.e upon clicking a button, call a `$.toast` function:

```html
<button class="toaster">Click me to toast!</button>

<script>
  $('.toaster').click(function(){
    $.toast({
      content: "I'm a toaster!"
    })
  })
</script>

```

#### hideAfter

If you'd like to have the toasts to not fade away, disable the `hideAfter` property

```html
<script>
  $.toast({
    content: "I'm a sticky toaster!",
    hideAfter: false
  })
</script>
```

#### Position

Changing the position of the toasts is done by setting the `position` property to one of the available position classes:

* `bottom-left`
* `bottom-right`
* `top-left`
* `top-right`

```html
<script>
  $.toast({
    content: "I'm a sticky toaster!",
    position: "bottom-left"
  })
</script>
```

### Stacking

Enable or disable stacking of toast elements

```html
<script>
  $.toast({
    content: "I won't stack!",
    stacking: false
  })
</script>
```

#### Embed HTML

You can even change the contents of the toast element to have other HTML elements


```html
<script>
  $('.toaster').click(function(){
    $.toast({
      content: '<i class="icon-warning"></i> <a href="/">Toaster link!</a>',
      position: "bottom-left"
    })
  })
</script>
```
