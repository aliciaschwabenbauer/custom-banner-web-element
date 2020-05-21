# custom-banner-web-element

This code snippet creates a custom privacy banner element and was created as part of a university course.

## Usage
As it is an npm package it can simply be importet with:
`npm install custom-banner-web-element`

### React 
In a react application(typescript) just:

```
# code block
import 'custom-banner-web-element'
...
//initialize an object reference 
const ref = createRef(); 
...

// add an event listener
const el: any = ref.current;
el.addEventListener('on-accept', () => {
    // callback function for whatever you want to do after accept is clicked
    setInteractionAllowed(classes.withInteraction)
    setBannerVisible(false); 
});

...
// render function in return staement(hooks)/render function with reference set from above 
<custom-banner 
          ref={ref} 
          application-name="Name"
          policy-link="Link">
</custom-banner>
```

### Other frameworks
For the usage in other frameworks, pleace refer to specific instructions

