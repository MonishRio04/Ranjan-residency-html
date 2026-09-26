# Ranjan Residency - Static Website (GitHub Pages Ready)

A modern, responsive luxury residency website for **Ranjan Residency, Vellore**, converted from Laravel to a pure HTML/CSS/JavaScript static application ready for deployment on **GitHub Pages**.

## 🌟 Highlights & Conversions

- **Zero Server / PHP Dependency**: Runs purely on static HTML, CSS, and client-side JavaScript.
- **Identical UI & Design**: 100% fidelity to the original design, colors, typography, Swiper carousels, GLightbox galleries, animations, and responsive mobile layouts.
- **Client & JS File-Based Data Operations**:
  - **Reviews System (`js/reviews-data.js`)**: All initial seeded reviews from `ReviewSeeder` are stored in JS. User review submissions are validated, stored in `localStorage`, and instantly rendered with flash success alerts.
  - **Media System (`js/media-data.js`)**: Media uploads, gallery highlights, and management portal operate client-side using HTML5 `FileReader` and browser storage.
  - **Site Data (`js/site-data.js`)**: Centralized data for rooms, amenities, nearby places, and gallery images.
- **GitHub Pages Compatible**: All asset links and navigation use relative paths, and `.nojekyll` is pre-configured to ensure all assets serve reliably.

---

## 📁 Project Structure

```text
├── index.html                  # Home page (Hero, Amenities, Rooms, Banquet, Ganesha, Highlights, Reviews)
├── about.html                  # About story & heritage
├── rooms.html                  # Rooms & suites showcase with Swiper sliders
├── vellore-sites.html          # Interactive nearby sites connection diagram & list
├── amenities.html              # Amenities & Mini A/C Convention Hall spotlight
├── gallery.html                # Prestige Photo Gallery with GLightbox lightbox
├── contact.html                # Contact information, Google Maps embed & quick call
├── ranjan-admin-portal.html    # Media upload & management portal
├── admin.html                  # Shortcut redirect to ranjan-admin-portal.html
├── .nojekyll                   # Disables Jekyll processing on GitHub Pages
├── css/
│   └── style.css               # Shared layout, color variables, typography, and responsive styles
├── js/
│   ├── main.js                 # Navigation toggle, active links, and lightbox initialization
│   ├── reviews-data.js         # JavaScript review database & relative time formatting
│   ├── media-data.js           # JavaScript media database & file upload handler
│   └── site-data.js            # Structured room, amenity, and location data
├── images/
│   └── site/                   # High-resolution residency images and room photos
└── uploads/                    # Uploaded media assets
```

---

## 🚀 How to Host on GitHub Pages

1. **Push this repository to GitHub**:
   ```bash
   git init
   git add .
   git commit -m "Convert Laravel project to static HTML for GitHub Pages"
   git branch -M main
   git remote add origin https://github.com/<your-username>/<your-repo-name>.git
   git push -u origin main
   ```

2. **Enable GitHub Pages**:
   - Go to your repository on GitHub.
   - Click **Settings** > **Pages** (under the "Code and automation" section).
   - Under **Build and deployment** > **Source**, select **Deploy from a branch**.
   - Under **Branch**, select `main` and folder `/ (root)`.
   - Click **Save**.

3. **Visit Your Live Website**:
   GitHub will deploy your website to `https://<your-username>.github.io/<your-repo-name>/`.

---

## 💻 Local Testing & Preview

To preview the project locally, you can:
- **Directly open** `index.html` in any modern web browser (Google Chrome, Microsoft Edge, Safari, Firefox).
- Or run any local static HTTP server:
  ```bash
  # Using Node.js (npx)
  npx serve .

  # Or using Python
  python -m http.server 8000
  ```
