# uiuctf-ctfd-theme

This is the official theme for UIUCTF! Follow the instructions below to install your theme. If there is anything that doesn't work please raise an **[issue](https://github.com/goelp14/uiuctf-ctfd-theme/issues/new/choose)**.

## Installation

As per https://docs.ctfd.io/en/latest/plugins.html and https://docs.ctfd.io/en/latest/themes.html you just have to do the following:
- Copy and paste the uiuctf theme folder into `/CTFd/themes`
- Replace `/CTFd/plugins/` with the one in this repository
- In the admin config tab (in your ctfd instance) you can upload the logo you want
    - You can find our logo in `/uiuctf/static/img/`
- You can update favicon in `/uiuctf/static/img` as well
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

## Creating and Modifying your own Version

The CTFd wiki doesn't really help too much in trying to make your own theme so I thought I would talk a bit about it. A lot of other community themes are not updated for the new version of CTFd so they break when you try to install them.

The cool thing to notice is that their core theme works completely so you can just copy that theme and modify that (or this one). I created a new css min and dev file in the static folder (since thats where its being pulled) to hijack the current css. You just need to add a reference to it in the main body (it extends to the rest of the template pages). If you are using this theme you can just edit `pranav.dev.css` and `pranav.min.css` (they need to have the same contents). Remember to hard reload to see changes appear. If you want to edit the css tags for challenges that is located in `challenges.js` in the assets folder. If you want to edit the challenge modal that appears you can find that in plugins. To see the changes for that you must empty cache ***AND*** hard reload. 

For more basic stuff you can change things on the actual website like I showed in the installation part of this README. Now you can restructure the HTML, add new classes, etc. Note that some things are served via JS so you may have to hunt around for those JS files and also add the classes there to gauruntee that they will actually render. For example there is a `challenges.min.js` and `challenges.dev.j` in the static js folder that you may need to edit too. It's a little bit annoying but it least it applies things across the theme (for the most part). 

That's pretty much it! I'm excited to see what you all do for future CTFs!

If you have any questions or want to get in contact with me my info is:

|Platform|Link|
|--------|----|
|Twitter|[@Etalerni](https://twitter.com/Etalerni)|
|Website|[pranavgoel.com](https://www.pranavgoel.com/)|

*Please also check out [UIUCTF](https://sigpwny.github.io/uiuctf) hosted by [SIGPWNY](https://sigpwny.github.io/)!*


​    
