# Krav Maga Edge website

The website for Krav Maga Edge, a self-defense academy in Hyderabad.

## Editing text and photos (no code)

The words and photos you are likely to change live in one file, `content/site.json`.
You edit it through a free visual editor, Pages CMS, with forms and drag-and-drop photos.
The design, layout and fonts stay exactly as they are.

**One-time setup**

1. Put this folder in a GitHub repository (on GitHub: **New repository**, then **Add file → Upload files** and drag in everything from this folder, including the `.pages.yml` file and the `content` and `img` folders).
2. In the repository, open **Settings → Collaborators** and add anyone else who should be able to edit.
3. Open **Settings → Pages**, choose **Deploy from a branch**, branch `main`, folder `/ (root)`, and save. GitHub shows the site's address a minute later.
4. Go to https://app.pagescms.org, click **Sign in with GitHub**, allow access to this repository, and open it.

**Every time you want to change something**

1. Open https://app.pagescms.org and pick the repository.
2. Click **Website text & photos**.
3. Click into any box and type, or drag a photo onto a photo box. Use **Add** and the bin icon to add or delete gallery photos, testimonials, events and blog posts.
4. Click **Save**. The live site updates within a couple of minutes (refresh the page to see it).

What you can edit there:

- **Every heading, paragraph, button, link, list item and photo on every page**, under "All text, buttons and sections". Each field is labelled with the text it currently shows, so you can find it quickly. Put words in [square brackets] to show them in red, and press Enter for a line break.
- **Show or hide any section** with its "Show this section" tick box.
- **Colours and font:** the brand red, background colour, text colour and the font, under "Colours and font".

The quick-edit groups below are still there for the most common changes:

- Home page headline, the line above it, the text below it, and the background photo
- The numbers (clients, corporate employees, years, others trained)
- Instructor name, photo, short description, profile points and years
- About page photo gallery (add, remove, reorder, replace)
- Client testimonials
- Events and blog posts (each with a title, date, text, optional photo and link)
- WhatsApp number, Instagram, Facebook and YouTube links (leave YouTube empty to hide its icon)
- Footer text

Every save is kept in the repository's history, so any change can be undone.

## Other files

- `index.html`: the page itself (design and layout). The text in it is the fallback if `content/site.json` can't load.
- `img/`: photos. New photos added in the editor are stored here.
- `hero-logo.mp4`, `hero-logo.webm`: the logo animation.
- `.pages.yml`: the editor's settings (which fields appear in the forms).

For developers: each editable element in `index.html` has a `data-t`, `data-ti` or `data-sec` key that matches an entry under `pages` in `content/site.json`. If you add or move elements in `index.html`, check the keys still match the content file.
