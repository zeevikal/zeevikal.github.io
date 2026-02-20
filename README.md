# zeevikal.github.io

Personal academic website for Zeev Kalyuzhner, built with Jekyll and deployed on GitHub Pages.

## Quick Start

### Local Development

```bash
bundle install
bundle exec jekyll serve
```

Then open [http://localhost:4000](http://localhost:4000).

### Deploy to GitHub Pages

1. Push this repo to `github.com/zeevikal/zeevikal.github.io` (the `master` branch).
2. Go to **Settings > Pages** and set source to the `master` branch.
3. The site will be live at `https://zeevikal.github.io` within a few minutes.

## How to Update Content

### Add Your Profile Photo

1. Place your photo in `assets/images/profile.jpg` (square crop, ~400x400px recommended).
2. The `index.html` header already references this path.

### Update Your CV PDF

Replace `files/cv.pdf` with your latest CV file.

### Add a New Publication

Edit `index.html` and add a new `<li>` inside the Publications `<ul class="pub-list">` section. Use `<span class="tag-new">New</span>` to highlight recent papers. Also update the highlight banner at the top if appropriate.

### Update Social / Academic Links

Edit the `.links` section in the header of `index.html`. Replace `YOUR_ID` in the Google Scholar URL with your actual Google Scholar profile ID.

### Change Accent Color

Edit `assets/css/style.css` and change the `--accent` CSS variable (default: `#e8590c` orange).

## File Structure

```
.
├── _config.yml          # Jekyll site configuration
├── _layouts/
│   └── default.html     # Base HTML layout
├── assets/
│   ├── css/
│   │   └── style.css    # All custom styles
│   └── images/
│       └── profile.jpg  # Your profile photo (add this)
├── files/
│   └── cv.pdf           # Your CV PDF
├── index.html           # Main single-page site content
├── Gemfile              # Ruby dependencies
└── README.md            # This file
```
