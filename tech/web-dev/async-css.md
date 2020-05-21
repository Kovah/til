# Async CSS

You can make CSS load in an async way by adding `media="print" onload="this.media='all'"` to the link tag. This will tell the browser
that these styles are less important, and thus will not block the rendering.

```html
<!-- Critical CSS, loaded first, blocks rendering -->
<link rel="stylesheet" href="main.css" />

<!-- Less important CSS, loaded later, does not block the rendering -->
<link rel="stylesheet" href="fonts.css" media="print" onload="this.media='all'" />
```

Source: [CSS Wizardry](https://csswizardry.com/2020/05/the-fastest-google-fonts/)
