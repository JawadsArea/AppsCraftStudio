# AppCraft Studio Website

The company website for **AppCraft Studio**, a studio that builds desktop apps, mobile apps and graphic design.

It is a single page made of one file, `index.html`. The HTML, CSS and JavaScript are all inside it, and the logo is embedded in it. There is nothing to install or build.

## Sections

The page scrolls through four sections, and the menu links jump to each one:

| Section | What it contains |
| --- | --- |
| **Home** | Hero with animated artwork, a scrolling services band, and the "How a project works" steps |
| **Services** | Desktop apps, mobile apps, UI/UX, graphic design, websites, support |
| **About** | Studio story, stats, and what the studio promises |
| **Contact** | WhatsApp, email and Facebook links, plus a contact form |

## What we offer

- **Desktop apps:** Windows only for now.
- **Mobile apps:** Android and iOS.
- **Graphic design and UI/UX design.**
- **Websites:** business sites and landing pages.
- **Support:** bug fixes and new features.

Not offered yet: Linux and macOS apps, publishing apps to stores, hosting setup, performance checks.

## Contact details used on the site

- WhatsApp: <https://wa.me/923447004147>
- Email: accesstojawadahmed@gmail.com
- Facebook: <https://www.facebook.com/AppsCraftStudios>

The contact form does not use a server. "Send on WhatsApp" opens WhatsApp with the message filled in, and "Send by email" opens the visitor's email app.

## Publish it free on GitHub Pages

1. Create a new repository on GitHub, for example `appcraftstudio`.
2. Upload `index.html` (and this `README.md`) to the repository. Keep the file name `index.html`.
3. Go to **Settings → Pages**.
4. Under **Branch**, choose `main` and `/ (root)`, then click **Save**.
5. After a minute the site is live at `https://YOUR-USERNAME.github.io/appcraftstudio/`.

To use your own domain, add it under **Settings → Pages → Custom domain**.

## Edit the site

Open `index.html` in any text editor. The code is split into clearly commented parts.

- **Services and text:** search for the section comments such as `SERVICES`, `ABOUT` and `CONTACT` in the HTML.
- **Hero phrases:** edit the `phrases` list in the script, under "Hero phrase rotation".
- **Colors:** change the values at the top of the CSS under `:root`.
- **Scrolling band words:** edit the `labels` list in the script, under "Scrolling text band".
- **About stats:** the numbers use `data-count` in the About section. The "24h typical first reply" figure is a placeholder, so change it to match your real reply time.
- **Logo:** the logo is stored inside `index.html` as base64 PNG images. The browser-tab icon is a small navy square version (in the `<link rel="icon">`), and the header uses a transparent version of the logo (the white gear with `</>`, the purple gear and the brush). To replace them, convert your new logo to base64 and swap the text after `data:image/png;base64,` in both places.
- **Color balance:** the colors come from the logo and follow a 60/30/10 split. Navy `#09123d` is the main color (about 60%), purple `#6f54c5` is the second color (about 30%), and white is the accent (about 10%). Change the values under `:root` to adjust it.

## Features

- Responsive layout for phones, tablets, laptops and large monitors
- Hamburger menu on small screens
- Hero with animated gears, window, phone and paintbrush that move slightly with the mouse
- Particle background and scrambled-text phrase in the hero
- Scrolling services band that speeds up as you scroll
- Menu link highlights the section you are viewing
- Animations switch off for visitors who have "reduce motion" turned on

The animated effects are written in plain HTML, CSS and JavaScript. They are inspired by [React Bits](https://reactbits.dev) but do not use its code.

## Notes

- The fonts (Montserrat and Inter) load from Google Fonts. If they cannot load, the page falls back to the visitor's system fonts.
- No cookies, trackers or other external scripts are used.
