# uiuctf-ctfd-theme
## Installation

As per https://docs.ctfd.io/en/latest/plugins.html and https://docs.ctfd.io/en/latest/themes.html you just have to do the following:
- Copy and paste the uiuctf theme folder into /CTFd/themes
- Replace /CTFd/plugins/ with the one in this repository
- In the admin config tab (in your ctfd instance) you can upload the logo you want
    - You can find our logo in /uiuctf/static/img/
- Update the CSS head in the admin config with the following code

```css
<style id="theme-color">
:root {--theme-color: #71B5FB;}
.navbar{background-color: var(--theme-color) !important;}
.jumbotron{background-color: var(--theme-color) !important;}
  font-family: 'FinkHeavy'!important;
</style>
```

-   Update index html by doing the following

    -   Click on Admin Panel
    -   Click on Pages -> All Pages
    -   Click on Index
    -   Copy and paste the following HTML as content
    -   Feel free to change things up as you like in the HTML


 ```html
    <div class="row">
        <div class="col-md-6 offset-md-3">
            <img class="w-100 mx-auto d-block" style="max-width: 500px;padding: 50px;padding-top: 14vh;" src="themes/uiuctf/static/img/uiuctf-logo.png" />
            <h3 class="text-center">
                <a href="https://sigpwny.github.io/uiuctf">UIUCTF Info</a>
                <p>Follow us on social media:</p>
                <a href="https://twitter.com/sigpwny"><i class="fab fa-twitter fa-2x" aria-hidden="true"></i></a>&nbsp;
            </h3>
            <br>
            <h4 class="text-center">
                <a href="https://discord.gg/PytGqjq" target="_blank" rel="noreferrer noopener">Click here</a> to join our Discord!
            </h4>
        </div>
    </div>
 ```

​    
