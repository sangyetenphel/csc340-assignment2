# Marvel Heroes & Villains

A responsive, multi-page website that showcases superheroes and villains, built with HTML, CSS, Bootstrap 5 and a little JavaScript for CSC 340 at UNC Greensboro, Assignment 2.

## Pages

| Page | File | What it shows |
|---|---|---|
| Home | `index.html` | A searchable grid of character cards (Iron Man, Doctor Doom, Batman, Deadpool and Hulk), each with an image, universe, role, species, power level and a short description |
| Character Details | `details.html` | A full profile for Iron Man: a banner image, his backstory, abilities and a details card |
| About Us | `about.html` | Why the site was built around Marvel characters, and the design approach |
| Add a Character | `new-character-form.html` | A form to submit a new character: name, universe (Marvel or DC), role, image upload and description |

## Features

- **Live search:** on the home page, typing a name or a category such as "hero", "villain", "human" or "dc" filters the cards. Press Enter or click Search, and a "no results" message appears when nothing matches. Clearing the box shows every card again.
- **Responsive layout:** Bootstrap's grid shows one card per row on phones and three per row on wider screens, and the navigation bar collapses into a menu on small screens.
- **Consistent navigation:** every page shares the same navbar, with a dropdown of characters and the current page highlighted.
- **Card styling:** custom CSS crops the character images to the same size and lifts each card slightly on hover.

## How the search works

Each card has a `data-name` attribute holding search keywords (for example `"iron man tony stark hero avenger human technology marvel"`). The script in `index.html` lowercases the search text, hides every card whose keywords don't contain it, and toggles the "no results" message.

## Project structure

```
index.html                Home page with the character cards and search
details.html              Iron Man character profile
about.html                About the website
new-character-form.html   Add-a-character form
img/                      Character images and logos
```

## Running it locally

No installation is needed: open `index.html` in a browser. Bootstrap loads from the jsDelivr CDN, so an internet connection is needed for the styling.

## Limitations

This is a front-end-only site, so:

- the Add a Character form checks that the required fields are filled in, but doesn't save anything;
- every entry in the Character Details dropdown opens the Iron Man page, which is the only details page so far.

## Built with

- HTML5 and CSS3
- [Bootstrap 5.3](https://getbootstrap.com/) for the layout, navbar, cards and form styling
- JavaScript for the character search

Character images are used for educational purposes only. Marvel and DC characters are trademarks of their respective owners.

Created by Sangye Tengkhar, February 2026.
