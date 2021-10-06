# Bootstrap
Do not add margin or padding left and right until inside the "col"

Do not add detail to the row without having a col

Order class- container: row: col
in a col can add- row: col's inside

https://getbootstrap.com/docs/5.1/getting-started/introduction/

<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.2/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-uWxY/CJNBR+1zjPWmfnSnVxwRheevXITnMqoEIeG1LJrdI0GlVs/9cVSyPYXdcSF" crossorigin="anonymous">

changes the display on mobile to not show a specific item- d-none d-md-flex

card spill- .card-spill{ transform: translateY(15px)}

media queery (make the card not spill on mobile)(min is greater than max is less than)- 
@media only screen and (min-width:768px){
.card-spill{
transform: translateY(15px)
}
}