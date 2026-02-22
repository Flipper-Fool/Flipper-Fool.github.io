# classless blog

This is a hugo-theme for blogs.

It is extremly minimalistic and only features standard html - no javascript or custom css.
This makes it very accessible, responsive and privacy friendly (there is no tracking at all).

To make it also *look good* a classless-css framework can be included.

## Demo

A [demo of this theme](https://kaligule.gitlab.io/classless-blog) (with the default "Water.css" framework) is hosted on Gitlab pages.

## Choose a framework

Some cool classess-css frameworks are:

- [Water.css](https://watercss.kognise.dev/)
- [Classless.css](http://classless.de/)
- [Sakura](https://oxal.org/projects/sakura/)
- [Marx](https://mblode.github.io/marx/)
- [AtriCSS](https://raj457036.github.io/attriCSS/)

But there are many more out there.

## Use a framework

Such classess-css frameworks provide stylesheets that can be included into this theme in two ways, both with different pros and cons:

### Via url in the config

Add an url to a stylesheet into your sites config like this:

In your `config.yaml`:
```yaml
params:
  stylesheetUrl: "https://unpkg.com/sakura.css/css/sakura.css"
```

Or in your `config.toml`:
```yaml
[params]
stylesheetUrl = "https://unpkg.com/sakura.css/css/sakura.css"
  ```

##### Pros

- little effort
- small diffs when changing the framework
- will update automatically if the framework is updated

##### Cons

- you are dependend on a third party, which might go down without notice
- the third party might track your users

### File in `static/css/`

Download the stylesheet and put it into the sites static folder as `static/css/stylesheet.css`.
If this file exists then the option `stylesheetUrl` from the config will be ignored.

##### Pros

- full controll over what is part of your site
- you can overwrite the file if you want
- you can use your own stylesheets, even if they are not publicly available
- you can get creative with using _git submodules_ or _makefiles_ to automate the process

##### Cons

- changing frameworks is more work
- foreign css-code is now in your repo

## Custom parameters

There is only one standard parameter for posts: If you want a cover image, add it like this:

```yaml
image: path/to/image.jpg
```

Most of the time the path will just be `coverimage.jpg` or so.
This assumes that your posts are organized as page-bundles (which is the most sensible way anyways).
Have a look at the exampleSite  to see how this would look.

## Ideas for improvement

- Add ci tests
- Automatically create Screenshots in the CI
- Have versions of the demo site online for different css-frameworks
- Make sure the project can be internationalized well
