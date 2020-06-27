# uiuctf-ctfd-theme
## Installation

As per https://docs.ctfd.io/en/latest/plugins.html and https://docs.ctfd.io/en/latest/themes.html you just have to do the following:
- Copy and paste the uiuctf theme folder into /CTFd/themes
- Replace \CTFd\plugins\ with the one in this repository
- In the admin config tab (in your ctfd instance) you can upload the logo you want
- Update the css in the admin config with the following code

```css
<style id="theme-color">
:root {--theme-color: #71B5FB;}
.navbar{background-color: var(--theme-color) !important;}
.jumbotron{background-color: var(--theme-color) !important;}
  font-family: 'FinkHeavy'!important;
</style>
```

