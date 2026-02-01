# JACKINone boot screen template

<div align="center">

**a modern, animated boot screen template with niiice visual effects**

![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)
![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=flat&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/css3-%231572B6.svg?style=flat&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=flat&logo=javascript&logoColor=%23F7DF1E)

</div>

## quick start

1. **download** the `index.html` file
2. **customize** your SVG assets (see customization guide below)
3. **open** `index.html` in any modern browser
4. **enjoy** your new boot screen.
5. **add** to any project of yours.

---

## file structure

```
JACKINone/
├── index.html              # main template file
├── symbol.svg             # central boot logo
├── gradient.svg           # background gradient
├── loading/ 
│   ├── loadingdone.svg    # final loading state
├── social-cards/
│   ├── email.svg          # default email card
│   ├── emailhover.svg     # email card hover state
│   ├── threads.svg        # default threads card
│   ├── threadshover.svg   # threads card hover state
│   ├── instagram.svg      # default instagram card
│   └── instagramhover.svg # instagram card hover state
└── README.md              # this file
```

---

## customization guide

### 1. **replace your logo**
Upload your own `symbol.svg` (recommended size: 134×123px) yes, it's odd. just get copilot to resize.

### 2. **create custom social cards**
edit your social cards using my figma template:

**[get social cards template →](https://www.figma.com/community/file/1599595673268266006)**

export your designs as SVG files and replace:
- `email.svg` & `emailhover.svg`
- `threads.svg` & `threadshover.svg` 
- `instagram.svg` & `instagramhover.svg`

### 3. **customize colors & timing**

edit the CSS variables in `index.html`:

```css
:root {
    --bg-primary: #0A0A0A;     /* main background */
    --text-primary: #ffffff;   /* text color */
    --accent: #0a84ff;         /* accent color */
}
```

adjust animation timings:

```css
animation: breatheIn 0.6s cubic-bezier(0.175, 0.885, 0.32, 1.275) forwards;
```

### 4. **update social links**

in the HTML section, update the data attributes:

```html
<div class="social-card email-card" data-email="your-email@example.com">
<div class="social-card threads-card" data-url="https://threads.net/@yourusername">
<div class="social-card instagram-card" data-url="https://instagram.com/yourusername">
```

## advanced configuration

### animation timing

| phase | duration | description |
|-------|----------|-------------|
| entry | 0.6s | elements breathe in |
| display | 9.4s | interactive phase |
| exit | 1s | fade to black |
| welcome | 1s | welcome screen fade in |

### social card interactions

- **email card**: copies email to clipboard on click.
- **social cards**: opens links in new tab.
- **hover effects**: smooth image transitions.

## technical details

**built with:**
- pure HTML5, CSS3, and vanilla JavaScript.
- CSS Grid & Flexbox for responsive layouts.
- CSS Custom Properties for easy theming.
- modern animation techniques with cubic-bezier timing.

---

## contributing

found a bug or want to suggest an improvement? feel free to:

1. fork the repository
2. create your feature branch
3. submit a pull request

---

## credits

**created by Noir** - a white label template, use as you wish! ❤️


</div>
