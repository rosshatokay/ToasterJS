# toasterjs
Create toaster notifications with a single line of code.

For quick examples and demos, head to [toasterjs.github.com](https://toasterjs.github.com/).

## Installation

You can install toasterjs from a hosted version on [cdnjs](https://www.npmjs.com/package/jquery-modal):

```html
<!-- Remember to include jQuery :) -->
<script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.0.0/jquery.min.js"></script>

<!-- jQuery Modal -->
<script src="https://cdnjs.cloudflare.com/ajax/libs/jquery-modal/0.9.1/jquery.modal.min.js"></script>
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/jquery-modal/0.9.1/jquery.modal.min.css" />
```

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

#### Make them stick
If you'd like to have the toasts to not fade away, disable the `hideAfter` property

```html
<script>
  $.toast({
    content: "I'm a sticky toaster!",
    hideAfter: false
  })
</script>
```
