---
# try also 'default' to start simple
theme: seriph
download: true
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
background: https://source.unsplash.com/collection/94734566/1920x1080
# apply any windi css classes to the current slide
class: 'text-center'
# https://sli.dev/custom/highlighters.html
highlighter: shiki
# show line numbers in code blocks
lineNumbers: false
# some information about the slides, markdown enabled
info: |
  ## Slidev Starter Template
  Presentation slides for developers.

  Learn more at [Sli.dev](https://sli.dev)
# persist drawings in exports and build
drawings:
  persist: false
---

# Tailwind CSS

Crash Course for Developers

<div class="pt-12">
  <span @click="$slidev.nav.next" class="px-2 py-1 rounded cursor-pointer" hover="bg-white bg-opacity-10">
    Press Space for next page <carbon:arrow-right class="inline"/>
  </span>
</div>

<div class="abs-br m-6 flex gap-2">
  <button @click="$slidev.nav.openInEditor()" title="Open in Editor" class="text-xl icon-btn opacity-50 !border-none !hover:text-white">
    <carbon:edit />
  </button>
  <a href="https://github.com/slidevjs/slidev" target="_blank" alt="GitHub"
    class="text-xl icon-btn opacity-50 !border-none !hover:text-white">
    <carbon-logo-github />
  </a>
</div>

---
layout: image-right
image: https://images.unsplash.com/photo-1558021211-6d1403321394?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=2465&q=80
---

<div>
  <div class="max-w-7xl mx-auto py-16 px-4 sm:py-24 sm:px-6 lg:px-8">
    <div class="text-center">
      <h2 class="text-base font-semibold tracking-wide uppercase">3 things</h2>
      <p class="pt-3 text-4xl font-extrabold">To keep in mind</p>
      <p class="max-w-xl pt-6 mx-auto text-xl text-gray-400">when learning anything new.</p>
    </div>
  </div>
</div>

---
layout: image-left
image: https://images.pexels.com/photos/2346289/pexels-photo-2346289.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=2
class: 'text-white'
---

# Don't compare yourself to others

<br>

<!-- <ul>
  <li>We are all different and here for different things</li>
  <li>We're all good at different things</li>
  <li>We all learn different things at different paces</li>
</ul> -->

---
layout: image-left
image: https://images.pexels.com/photos/3791136/pexels-photo-3791136.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=2
class: 'text-white'
---

# If you're tired of starting over stop giving up 

---
layout: image-left
image: https://images.pexels.com/photos/7210670/pexels-photo-7210670.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=2
class: 'text-white'
---

# The obstacle is the way

<br>

---
layout: image-right
image: https://cdn.dribbble.com/users/25514/screenshots/15344343/media/1c5c9f6ce8f9817ca1740cc44a1df199.png?compress=1&resize=400x300
---

# What is a Design System?

<br>

A design system is “everything that makes up your product”.

From typography, layouts and grids, colors, icons, components and coding conventions, to voice and tone. 

A design system is bringing all of these together to make building things on the web faster, better, and easier.



<br>
<br>

---
class: px-20 pt-20
layout: image-left
image: https://miro.medium.com/max/700/1*Ceq9JteKuwBdBwkbsUriQw.png
---

# Why Tailwind?

Tailwind CSS has the highest satisfaction rate among the developers who had the opportunity to work with it. Source: “The State of CSS 2019”

1 - It is Highly Customizable <br>

2 - It Has Common Utility Patterns <br> 
<!-- No more naming classes -->
3 - It Can Be Optimized <br>
<!-- PurgeCSS -->
4 - Complex Responsive Layouts <br>
<!-- (Mobile First) -->
5 - All in one place <br>


<style>
h1 {
  background-color: #2B90B6;
  background-image: linear-gradient(45deg, #4EC5D4 10%, #146b8c 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent; 
  -moz-text-fill-color: transparent;
}
</style>

---

# What is Tailwind CSS?

Tailwind CSS is a highly customizable, Low Level CSS framework. 
It provides you with a huge set of utility classes to build
your own components and not just a set of predefined/prebuilt components.
Such is the case of Bulma, Bootstrap, Material UI or other CSS frameworks.

- 📝 **Utility-based** - Provides you with pre defined classes or shortcuts.
- 🎨 **Themable** - Theme can be shared and used dynamically.
- 🧑‍💻 **Developer Friendly** - Enables you to have all style and markup in one single file.
- 🤹 **Responsive** - Provides mobile first utilities out of the box.
- 📤 **Lightweight** - It's fast, flexible, and reliable — with zero-runtime.
- 🛠 **Hackable** - Anything possible and customizable. 

<br>
<br>

Read more about [Why Tailwind?](https://tailwindcss.com/)

<!--
You can have `style` tag in markdown to override the style for the current page.
Learn more: https://sli.dev/guide/syntax#embedded-styles
-->

<style>
h1 {
  background-color: #2B90B6;
  background-image: linear-gradient(45deg, #4EC5D4 10%, #146b8c 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent; 
  -moz-text-fill-color: transparent;
}
</style>

---

# Installation

Tailwind CSS works by scanning all of your HTML files, JavaScript components, and any other templates for class names, generating the corresponding styles and then writing them to a static CSS file.

### Install via npm, and create your `tailwind.config.js` file.

#

```
npm install -D tailwindcss
npx tailwindcss init
```

#

### Add the @tailwind directives for each of Tailwind’s layers to your main CSS file.

#

```javascript
@tailwind base;
@tailwind components;
@tailwind utilities;
```

---
layout: image-right
image: https://source.unsplash.com/collection/94734566/1920x1080
---

# Run the CLI tool.

Scan your template files for classes and build your CSS.

```
npx tailwindcss -i ./src/input.css -o ./dist/output.css --watch
```

#

### Start using Tailwind in your HTML

```html
<!doctype html>
<html>
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <link href="/dist/output.css" rel="stylesheet">
</head>
<body>
  <h1 class="text-3xl font-bold underline">
    Hello world!
  </h1>
</body>
</html>
```


---

# Colors

<div grid="~ cols-2 gap-4">
<div>

Tailwind gives you shortcuts to access pre defined colors 
or it let's you create your own theme and access the aliased colors 
from your template.

### Background Color 

```javascript
<button class="bg-indigo-500 ...">
  Save changes
</button>
```

#

<button class="bg-indigo-500 text-white p-2">
  Save changes
</button>

#

### Text Color 

```javascript
<p class="text-red-600">Tailwind is awesome!</p>
```

#
<p class="text-red-600">Tailwind is awesome!</p>


Check out [the guides](https://tailwindcss.com/docs/background-color) for more.

</div>
<div>

Or you can create your own custom layout

```javascript
module.exports = {
  theme: {
    extend: {
      colors: {
        'regal-blue': '#243c5a',
      },
    }
  }
}
```

and reference it from the template tag.

```javascript
<p class="text-regal-blue">
  Lorem Ipsum
</p>
```


</div>
</div>

---
class: px-20
---

# Spacing, Margin and Padding

Control the margin on one side of an element using the m{t|r|b|l}-{size} utilities.

<div grid="~ cols-2 gap-2">

```javascript
m-0	| margin: 0px;
mt-0 | margin-top: 0px;
mr-0 | margin-right: 0px;
mb-0 | margin-bottom: 0px;
ml-0 | margin-left: 0px;
```

</div>

<div grid="~ cols-2 gap-2" m="-t-2">

Utilities for controlling an element's padding.

#

```javascript
p-0	| padding: 0px;
pt-0 | padding-top: 0px;
pr-0 | padding-right: 0px;
pb-0 | padding-bottom: 0px;
pl-0 | padding-left: 0px;
```

</div>

Read more about [How to use spacing](https://tailwindcss.com/docs/customizing-spacing).

---
class: px-20
---
# Width and Height

You can also setup an elements Width, Height, minimum width/height, or maximum width/height and so on.

### Fixed width

```javascript
<div class="w-48 ..."></div>
<div class="w-40 ..."></div>
<div class="w-32 ..."></div>
<div class="w-24 ..."></div>
```
### Percentage width

```javascript
<div class="flex ...">
  <div class="w-1/2 ... ">w-1/2</div>
  <div class="w-1/2 ... ">w-1/2</div>
</div>
<div class="flex ...">
  <div class="w-1/5 ...">w-1/5</div>
  <div class="w-4/5 ...">w-4/5</div>
</div>
```

---

# Hover, Focus, and Other States

<br>

Every utility class in Tailwind can be applied conditionally by adding modifier to the beginning of the class name that describes the condition you want to target.

For example, to apply the bg-sky-700 class on hover, use the hover:bg-sky-700 class.

<div class="grid grid-cols-2 gap-10 pt-4 -mb-6">

```javascript
<button class="bg-sky-500 hover:bg-sky-700 ...">
  Save changes
</button>
```

<button class="bg-sky-500 hover:bg-sky-700 ...">
  Save changes
</button>


```javascript
<button class="bg-fuchsia-200 hover:bg-fuchsia-600 ...">
  Save changes
</button>
```

<button class="bg-fuchsia-200 hover:bg-fuchsia-600 ...">
  Save changes
</button>

<br>
</div>

[Learn More](https://tailwindcss.com/docs/hover-focus-and-other-states#hover-focus-and-active)

---

# You can also create your own utility classes!

One of the best parts of using Tailwind is defining your own utility functions.

I recently needed a negative z-index, but Tailwind doesn't have one, so I created my own:

```javascript
@layer utilities {
  .-z-1 {
    z-index: -1;
  }
}
```

Anything wrapped with @layer utilities { ... } will be picked by Tailwind as a utility class.

This lets you write `md:-z-1 lg:z-0` and have the utility class respond to screen size.

### It's super simple!

---
layout: center
class: text-center
---

# Flexbox, Grid, Transforms, Fonts, Borders, Shadows...

...or any design you want!

[Documentation](https://tailwindcss.com/) · [TailwindUI](https://tailwindui.com/) · [Traversy Media Crash Crouse](https://www.youtube.com/watch?v=UBOj6rqRUME)

---
layout: center
class: text-center
theme: seriph
background: https://source.unsplash.com/collection/94734566/1920x1080
---

# Thank you!

