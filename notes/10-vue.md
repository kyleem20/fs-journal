# VUE
Day 1: https://github.com/BoiseCodeWorks/late-fall21-slap
Day 2: https://github.com/BoiseCodeWorks/late-fall21-vueflix
Fireside: https://github.com/JustinCarpenter2020/lateFall21-vuePokedex


(optional) vpm i @vue/next

es lint: eslintrc.js : change singleline to different number (restart vs code to update file)

export default: generally should not need to use this.___ to call a function

any variable you want in your template must be returned in your template

in script: need function.value (value is key) where you change the function's value when you call it
in style: .value is implied

props are data passed from parent component to child component

components act as the controller
.vue is a single file component
v-if: doesn't put the html on the page
computed: vue's proxystate.on
v-for: repeats an element


Start with:
Initial Front Page Load up (navbar)
Router - connect to the Page
Set up API
Set up server
    -get/getId/create/edit/delete
Set up Page with mounted for "on click"


useRouter: where you are going
useRoute: where we are


router links go inside the template, params called in the router file; utility/functionality
information out of url into script tag: get the route from useRoute; details
router.push: brings back to the home page

.push: adds to end of array
.unshift: adds to the beginning of array

findoneUpdate



When to use:
onMounted- when page loads,
watchEffect-
computed-