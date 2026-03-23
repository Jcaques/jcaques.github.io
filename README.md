# My Portfolio

A clean, minimal portfolio website built with plain HTML/CSS/JS — no dependencies, no build step. Hosted with [GitHub Pages](https://pages.github.com).

## 🚀 Deploy to GitHub Pages

1. **Create a new repo** named `yourusername.github.io` on GitHub  
   (Replace `yourusername` with your actual GitHub username)

2. **Clone it locally:**
   ```bash
   git clone https://github.com/yourusername/yourusername.github.io
   cd yourusername.github.io
   ```

3. **Copy your files in:**
   ```bash
   cp /path/to/index.html .
   ```

4. **Push to GitHub:**
   ```bash
   git add .
   git commit -m "Initial portfolio"
   git push origin main
   ```

5. **Done!** Your site will be live at `https://yourusername.github.io` within a minute or two.

---

## ✏️ Customizing the Site

### Personal Info
Open `index.html` and search/replace these placeholders:

| Placeholder | Replace with |
|---|---|
| `YourName` | Your display name (nav logo) |
| `Your Name` | Your full name (hero & about) |
| `[Your City]` | Your location |
| `hello@yourname.dev` | Your email |
| `yourusername` | Your GitHub handle |

### Projects
Find the `<!-- PROJECTS -->` section and duplicate a `.project-card` block for each project. Update:
- The emoji in `.project-thumb` (or swap for an `<img>`)
- `.tag` chips with your tech stack
- `project-name` and `project-desc`
- The GitHub link in `project-link`

### Blog Posts
Find the `<!-- BLOG -->` section and add `.blog-post` entries. Each needs:
- A date and read time in `.blog-meta`
- A title in `.blog-title-link`
- An `href` pointing to your post (Markdown file, external link, etc.)

### Contact Form
The form currently uses a demo handler. To make it actually send emails:
1. Sign up at [Formspree.io](https://formspree.io) (free tier available)
2. Create a form and copy your form ID
3. Replace the `<form>` tag with:  
   `<form class="contact-form" action="https://formspree.io/f/YOUR_ID" method="POST">`
4. Remove the `<script>` block at the bottom

### Colors & Fonts
All theme values are CSS variables at the top of `<style>`:
```css
--accent: #2d6a4f;   /* green — change to any color */
--bg: #f9f7f4;       /* off-white background */
--ink: #1a1a18;      /* near-black text */
```
Swap `DM Serif Display` / `DM Sans` for any [Google Fonts](https://fonts.google.com) pair you prefer.

---

## 📁 File Structure

```
yourusername.github.io/
├── index.html        ← entire site lives here
├── resume.pdf        ← optional: add your resume
└── README.md
```

For blog posts you can add individual `.html` files (e.g. `blog/my-first-post.html`) and link to them from the blog section.
