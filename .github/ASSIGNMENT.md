# 📄 Vent Haven

Build a three-page website for the Vent Haven Museum, then style it with a flexbox navigation bar,
CSS grid layouts, a float, and background images.

## 🎯 Overview

Vent Haven Museum in Fort Mitchell, Kentucky, is the world's only museum of ventriloquist
figures. In this assignment you will turn the museum's text and photos into a three-page site:
a **Home** page, a **Berger Biography** page, and a **Dummy Spotlight** page. Every page shares
the same header, navigation bar, and footer; only the `main` content changes.

The videos walk you through the first parts: setting up the files, building the boxes, filling
them with content, and starting the styles. Then you finish the site **on your own** using the
checklist in [Part 5 — On Your Own](#-part-5--on-your-own).

This is one of the biggest assignments of the term, so start early. It's not something you can
finish the night before it's due.

> [!IMPORTANT]
> **The companion videos for this assignment are in Canvas**, on the assignment page. They walk
> you through Parts 1–4, so watch them there instead of working from this file alone.

## 🧠 What You Will Learn

By completing this assignment, you will practice how to:

- Build a multi-page site with a shared `header`, `nav`, and `footer`
- Link pages to each other with a navigation bar
- Turn a list of links into a horizontal navigation bar with Flexbox
- Lay out content in columns with CSS Grid
- Float an image so text wraps around it
- Use background images with `background-repeat`, `background-size`, and `background-position`
- Center a fixed-width wrapper and add borders and shadows

## 🎬 Watch the Videos in Canvas and Follow Along

The screencast videos are on this assignment's page in **Canvas**, not in this repo. Watch them
**in order** and follow along in your code editor. Pause whenever you need time to finish a
step — it is normal to pause, rewind, and rewatch parts of a coding demonstration.

| Video | What you will do |
| --- | --- |
| **Introduction & Overview** | See the finished site and how the starter files are organized. |
| **Part 1 — HTML Foundation & Boxes** | Create the home page and build the `wrapper`, `header`, `nav`, `main`, and `footer` boxes. |
| **Part 2 — Filling the Boxes** | Copy the header, navigation links, and footer text from `page_content_info.html` into the boxes. |
| **Part 3 — Marking Up the Main Content** | Add the page content and mark it up with headings, paragraphs, lists, and images, and create the other two pages. |
| **Part 4 — Styling** | Create your stylesheet, link it after `reset.css`, and start styling the site. |
| **Part 5 — On Your Own** | No video. Finish the site using the checklist [below](#-part-5--on-your-own). |

> [!IMPORTANT]
> **A few steps in this repo are different from the videos.** Follow the videos for the HTML and
> CSS, and follow this repo for getting your files and submitting:
>
> - **Getting the starter files:** don't download `venthaven_start.zip`. Create your own repo
>   from this template and clone it in WebStorm, as described in the
>   [Getting Started guide](GETTING_STARTED.md). The starter files are already in the root of your
>   repo, not in a `venthaven` folder.
> - **Naming your files:** the home page must be **`index.html`** in the root of the repo.
>   GitHub Pages only serves `index.html` at your site's root URL.
> - **Submitting:** don't zip your folder or upload a file. Publish your site to GitHub Pages and
>   submit a pull request URL in Canvas, as described in the
>   [Submitting guide](SUBMITTING.md).

## 📂 Starter Files

| File / Folder | Purpose |
| --- | --- |
| `page_content_info.html` | The text for every page: the header, nav link names, footer, and each page's `main` content. **Don't turn this into a web page.** Copy parts of it into the pages you create. |
| `reset.css` | Removes the browser's default styles. Link it on every page, **before** your own stylesheet. |
| `images/` | Photos of the museum and its dummies, plus the background images `bkg_head_black.png`, `bkg_head_white.png`, `bkg_footer.png`, and `bkg_column.jpg`. |

You create these pages (the videos show how):

| File | Page |
| --- | --- |
| `index.html` | Home |
| `berger.html` | Berger Biography |
| `dummy.html` | Dummy Spotlight (Featured Dummies) |

> [!NOTE]
> The checklist below calls the header images `bkg_header_black.png` and `bkg_header_white.png`.
> In the `images` folder they're named **`bkg_head_black.png`** and **`bkg_head_white.png`**. Use
> the names in the folder.

The `header`, `nav`, and `footer` are **exactly the same on every page**. Build them once, then
copy and paste them into the other pages.

## ✏️ Part 5 — On Your Own

The videos walk you through the first parts. Now apply what you've learned on your own, without
following along. Check off each box as you go.

### 🧭 Navigation Bar (all pages)

Add these rules to your stylesheet. They turn the unordered list of links into a navigation bar on
the right side of the header. (This recipe matches the *CSS for Navigation Bar Inside the Header*
page in your handout binder.)

```css
header {
  padding: 1em;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

nav {
  background-color: /* use any color you want */;
  padding: 1em;
  border-radius: 2em;
  font-size: 85%;
}

nav ul {
  list-style-type: none;
  display: flex;
  align-items: center;
}

nav a {
  padding: .5em 2em;
  text-transform: uppercase;
  text-decoration: none;
  color: /* use any color you want */;
}

nav a:hover {
  background-color: /* use any color you want */;
  border-radius: 2em;
  color: /* use any color you want */;
}
```

### 🎨 Styles for All Pages

| Selector | Styles to add |
| --- | --- |
| `body` | ☐ A `background-color`<br>☐ Change the font |
| `.wrapper` | ☐ A width of 960 pixels<br>☐ Center it on the page (left and right margins `auto`)<br>☐ A white background color<br>☐ A border<br>☐ A box shadow |
| `header` *(add to the nav bar rules above)* | ☐ A `background-color`<br>☐ At least `1em` of `padding` on all sides<br>☐ `bkg_head_black.png` or `bkg_head_white.png` as a `background-image` (p. 413 of your textbook)<br>☐ `background-repeat` so the image doesn't repeat<br>☐ `background-size: contain;`<br>☐ `background-position` to put it at the center left of the header |
| `header h1` | ☐ Increase the text size to `150%`<br>☐ A left margin so the text doesn't overlap the image<br>☐ *Optional:* change the color if you need more contrast with the background |
| `main` | ☐ Padding, with more on the left/right than the top/bottom<br>☐ `font-size: 125%;`<br>☐ `line-height: 1.4;` |
| `main h2` | ☐ Change the size<br>☐ A bottom border |
| `footer` | ☐ `bkg_footer.png` as a background image<br>☐ Center the text<br>☐ Padding on all four sides |
| `img` | ☐ Let images shrink to fit their containers: `max-width: 100%;` and `height: auto;` |

### 🏠 Home Page (`index.html`)

The home page's `main` is a two-column grid: an `about` section on the left and a narrower `visit`
column on the right.

```
div.wrapper
├── header
│   └── nav
├── main.home-grid
│   ├── section.about
│   └── section.visit
└── footer
```

**HTML**

- [ ] At least one image on the page (yours can be different from the example)
- [ ] A `class` attribute on the `<main>` element named `home-grid` (only on this page, not the
  other two)
- [ ] A new `<section class="about">` holding the first four paragraphs, ending **before** the
  *Visit Us* heading (Emmet: type `section.about` and press Tab)
- [ ] A new `<section class="visit">` holding the *Visit Us* heading and the remaining paragraphs
  in `main`

**CSS**

| Selector | Styles to add |
| --- | --- |
| `.home-grid` | ☐ Make it a grid container with `display`<br>☐ Two unequal columns: `grid-template-columns: 3fr 1fr;`<br>☐ A gap of `2em` with `grid-gap` |
| `.visit` | ☐ Reduce the text size to `90%`<br>☐ A `background-color`<br>☐ `1em` of `padding`<br>☐ Rounded corners with `border-radius`<br>☐ `bkg_column.jpg` as a background image<br>☐ Don't let the background image repeat<br>☐ `background-size: 70%;`<br>☐ `background-position: 50% 95%;`<br>☐ *Optional:* if the background image overlaps the text, add some `padding-bottom` |

### 🎭 Dummy Spotlight Page (`dummy.html`)

```
div.wrapper
├── header
│   └── nav
├── main
│   └── section.dummy-grid
│       ├── section.red
│       └── section.jacko
└── footer
```

**HTML**

- [ ] The page `<title>` is *Vent Haven - Featured Dummies*
- [ ] Each dummy's picture is **above** the `h3` with their name
- [ ] A new `<section class="dummy-grid">` that starts **after the first paragraph** and holds
  everything about both dummies
- [ ] A `<section class="red">` with Red Flannels' picture, name, and list
- [ ] A `<section class="jacko">` with Jacko's picture, name, and list

```html
<section class="dummy-grid">
  <section class="red">
    <img src="images/red_flannels.jpg" alt="Red Flannels">
    <h3>Red Flannels</h3>
    <ul>
      <li>...</li>
    </ul>
  </section>
  <section class="jacko">
    <img src="images/jacko.jpg" alt="Jacko">
    <h3>Jacko</h3>
    <ul>
      <li>...</li>
    </ul>
  </section>
</section>
```

**CSS**

| Selector | Styles to add |
| --- | --- |
| `.dummy-grid` | ☐ Make it a grid container with `display`<br>☐ Two equal columns: `grid-template-columns: 1fr 1fr;`<br>☐ A `grid-gap` for room between the columns |
| `.dummy-grid img` | ☐ A 10 pixel white `border`<br>☐ A `box-shadow` |
| `.dummy-grid h3` | ☐ Increase the size<br>☐ Change the color<br>☐ A 1 pixel bottom border |
| `.dummy-grid li` | ☐ A `1em` margin on the bottom and left |

### 👤 Berger Biography Page (`berger.html`)

**HTML**

- [ ] One of the old pictures of William S. Berger on the page
- [ ] A `class` attribute on that image named `pic-right`

**CSS**

| Selector | Styles to add |
| --- | --- |
| `.pic-right` | ☐ `float: right;`<br>☐ A margin on the bottom and left<br>☐ A 10 pixel white `border`<br>☐ A `box-shadow` |

### 🔓 Solution Walkthrough Videos

There are walkthrough videos that show the correct way to do everything in Part 5, but they're
locked until you submit, so you don't see the answers before you try:

1. Finish the site on your own first.
2. Submit your pull request URL in Canvas.
3. The solution walkthrough module unlocks in Canvas.
4. Watch the videos to compare your work and troubleshoot.
5. If something is wrong, fix it on `develop` and push. Your open pull request updates
   automatically.

## 🧮 Grading

This assignment is worth **65 points**.

| Criteria | Full credit | Points |
| --- | --- | --- |
| **Files and pages** | `index.html`, `berger.html`, and `dummy.html` in the root, linked to each other from the nav | 6 |
| **Shared structure** | Every page has the same `div.wrapper`, `header`, `nav`, and `footer`, with content from `page_content_info.html` | 8 |
| **Main content markup** | Each page's content is marked up with headings, paragraphs, lists, and images | 8 |
| **Navigation bar** | The nav bar rules from Part 5, with your own colors and a hover state | 6 |
| **All-page styles** | `body`, `.wrapper`, `header` (with background image), `header h1`, `main`, `main h2`, `footer`, and `img` styled as listed | 14 |
| **Home page** | `main.home-grid` with `section.about` and `section.visit`, styled as a 3fr/1fr grid with the column background image | 9 |
| **Dummy Spotlight page** | Correct title; `section.dummy-grid` with `section.red` and `section.jacko`, styled as a two-column grid | 8 |
| **Berger Biography page** | A Berger photo with the class `pic-right`, floated right with margin, border, and shadow | 4 |
| **Published and submitted** | The site is live on GitHub Pages, and an open pull request with the live URL is submitted in Canvas | 2 |
| **Total** | | **65** |

## ✅ Before You Submit

- [ ] The home page is named `index.html` (not `index.html.txt`) and is in the root folder
- [ ] All three pages link to each other, and every nav link works on your live site
- [ ] `reset.css` is linked before your stylesheet on **every** page
- [ ] The header, nav, and footer are the same on every page
- [ ] Every box in Part 5 is checked off
- [ ] Every image loads on your live site (check upper and lower case in file names)
- [ ] The site is live on GitHub Pages and the URL is in your pull request

## 🛠️ Troubleshooting

- Did you save every file?
- **A nav link gives a 404?** Check that the `href` matches the file name exactly, like
  `berger.html`, and that the file is in the root folder.
- **Styles work on one page but not another?** Each page needs its own `<link>` to `reset.css`
  and your stylesheet.
- **Background image not showing?** Paths in CSS are relative to the CSS file. If your stylesheet
  is in the root, use `url(images/bkg_footer.png)`. Check the file name: it's `bkg_head_black.png`,
  not `bkg_header_black.png`.
- **Grid not working?** Check that the class in your HTML (`home-grid`, `dummy-grid`) matches
  your selector exactly, including the dot in CSS.
- **Text wrapping oddly around the Berger photo?** Make sure `pic-right` is on the `img`, and
  that the image comes before the paragraphs you want to wrap around it.

**Having problems with the videos?**

- **Getting a warning about third-party cookies?** Try using Chrome. Safari's default security
  settings may prevent embedded Canvas videos from playing unless those settings are changed.
- **Getting an "Access Denied" error?** Refresh your browser. In many cases, the videos will load
  correctly after the page reloads.

## 📚 Resources

- **Textbook:** background images (p. 413)
- Handout binder: *CSS for Navigation Bar Inside the Header*
- [MDN — Basic concepts of flexbox](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_flexible_box_layout/Basic_concepts_of_flexbox)
- [MDN — Basic concepts of grid layout](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_grid_layout/Basic_concepts_of_grid_layout)
- [MDN — `float`](https://developer.mozilla.org/en-US/docs/Web/CSS/float)
- [MDN — `background`](https://developer.mozilla.org/en-US/docs/Web/CSS/background)
- [W3C Markup Validation Service](https://validator.w3.org/#validate_by_input) — paste your HTML
  in to catch unclosed tags

## 🆘 Getting Help

Ask questions in class or during office hours, or send a message in Canvas. Include your live
GitHub Pages URL and your pull request URL so your instructor can see your code.

---

The AI policy and submission instructions are in the [README](../README.md).
