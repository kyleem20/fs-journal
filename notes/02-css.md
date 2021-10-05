# CSS
call a class="name" by using .name

variables in CSS: 
Example:
:root{
  --primary: #77a0a0
}

header {
  background-color: var(--primary)
}

Remove margin:
body {margin: 0}

Flexbox: formatting on page display
header{display: flex;
justify-content: space-evenly;}

Padding: 2em; <-adds padding around children

object-fit: contain; <- forces image to fit correctly to the size you want, crops the photo (only works with a forced height and width)