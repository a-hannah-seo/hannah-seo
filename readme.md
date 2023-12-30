# overview
this website is built with the templating framework Jekyll, with a modified Minima theme. the deployment service, Netlify, listens to changes to the main branch and automatically builds and deploys the site.

overrides to the Minima theme are provided by explicitly providing our own version of the theme files in the project. for example, we inject our own css by copying the `_sass/minima.scss` file from the theme package and adding our own `@import`s of our css files.

## pages
the top-level pages consist of a `.md` or `.html` template. the former is fed by data in `.yml` files.

| page | file/template | template data source | notes |
|---|---|---|---|
| / | `/index.md` || top level homepage
| /audio | `/pages/audio.md` | `_data/clips.yml` |
| /contact | `/pages/contact.md`  || contact form, powered by Netlify
| /journalism | `/pages/journalism.md` | `_data/articles.yml`
| /poetry | `/pages/poetry.md` | `_data/poems.yml`
| /thanks | `/pages/thanks.html` || contact form's post-submit landing page
| /* | `/404.html` || 404 page

# making changes

## updating articles/clips/poems
since each page is a template, the external links on each of these pages can be modified by tweaking the page's corresponding `.yml` files. this can be done directly in the github in-browser editor. thanks to Netlify's auto-deploy pipeline, changes will be automagically reflected on the live site in less than a minute.

### step 1: upload an image
the current template design for the journalism and poetry pages use a background image (pulled from the article or poem itself).

1. download the image to your computer (and ideally, resize the image so it's < 200kb, to be nice to people using potatoes to look at your website. making it a `.jpg` or `.webp` would help, too).
	- name the file something simple, like `hypno.jpg`

2. navigate to the proper folder in the codebase:
	- [/assets/images/articles](https://github.com/a-hannah-seo/hannah-seo/tree/main/assets/images/articles)
	- [/assets/images/poems](https://github.com/a-hannah-seo/hannah-seo/tree/main/assets/images/poems)

3. on the top right, click `Add file -> Upload files` and drop your image file in
4. add a message (the default is "Add files via upload"... make it something nicer, like "add image for hypnosis article") and description (optional). 
5. click the big green button to `Commit changes` directly to the `main` branch.

voila, your file is uploaded.

### step 2: open the editor
the below links will open up with in-browser editors for their corresponding data files:
- [🔗 edit /audio clips (clips.yml)](https://github.com/a-hannah-seo/hannah-seo/edit/main/_data/clips.yml) 
- [🔗 edit /journalism articles (articles.yml)](https://github.com/a-hannah-seo/hannah-seo/edit/main/_data/articles.yml)
- [🔗 edit /poetry poems (poems.yml)](https://github.com/a-hannah-seo/hannah-seo/edit/main/_data/poems.yml)

### 3. make your changes (and don't explode the website)
make sure to use the existing data values and formats, following all pre-established patterns. it's also good practice to enclose the values to the right of the colon in double-quotes, like so:
```
- title: "What Can Hypnosis Do for Your Health?"
  publication: "The New York Times"
  blurb: "This 200-year-old treatment can be effective for a variety of conditions, but it does take work."
  link: "https://www.nytimes.com/2023/02/08/well/mind/hypnosis-therapy-mental-health-depression.html"
  image: "/assets/images/articles/hypno.webp"
  alt-text: "An illustration of a figure's head reflected left-right, with swirling hypnotic circles in between"
```

note that double quotes should only exist twice: in the beginning and the end of the value. for example, this will break:
 ```
- title: "Stop Calling It "Climate Anxiety." It's Climate Dread."
```
and these will work:
```
- title: "Stop Calling It 'Climate Anxiety.' It's Climate Dread."
```
```
- title: Stop Calling It "Climate Anxiety." It's Climate Dread.
```

### 4. save your changes
once you're done editing, click the big green `Commit changes...` button on the top right.

a window will pop up with the following fields:
- `commit message` — a one-liner summarizing your changes (convention is to use the present imperative tense: 'eat the vegetables', 'do the naenae', 'add a readme')
- `extended description` — more deets if you want to remember why you did this
- `commit email` — which email you want to use to sign your work
- and a radio button choice:
	- `commit directly to main branch` — this is fine for a small potatoes website like this
	- `create a new [...] pull request` — saves your changes to a temporary state for others to look over it and approve

for something as simple as updating data, the default choice for all of the fields above should be a-okay.

tap `Commit changes` and you're done! you'll see your latest commit in the commit history on the repository.

Netlify will pick up that there were changes, and it'll build and deploy them to the live website within a minute. 
