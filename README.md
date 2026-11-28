# Samir-Belgassab-final-project
# Her Haven — Safety, Dignity & Equality

A 3-page awareness website about violence against women with disabilities. It aims to share understanding, warning signs and ways to find support in a calm, respectful and accessible way.

## Project goals
- Raise awareness of the violence faced by women with disabilities.
- Explain why they face additional barriers and risks.
- Offer practical steps for seeking help safely.
- Stay respectful throughout: no graphic imagery, no invented numbers and no made-up information.

## Technologies used
- HTML5
- Css
- Tailwind CSS v4 (`@tailwindcss/browser` and `public/css/output.css`)
- DaisyUI 5 (navbar, menu and footer)

## Pages
| Page | File | Content |
| --- | --- | --- |
| Home | `index.html` | Hero, "Why it matters" (3 cards), quote and call to action |
| Understanding Violence | `public/pages/about.html` | 6 forms of violence, warning signs, illustrative scenarios and rights |
| Help & Support | `public/pages/contact.html` | 4 safe steps, safety checklist, friends and family, resources and a contact form |

## How to run the project
1. Clone the repo:
   ```bash
   git clone <repo link>
   ```
2. Open `index.html` in a browser. An internet connection is needed because DaisyUI and Tailwind load from a CDN.
3. If you change classes and want to rebuild `output.css` with the Tailwind CLI:
   ```bash
   npx @tailwindcss/cli -i <input.css> -o ./public/css/output.css --watch
   ```
   (replace `<input.css>` with your own input file)

## Structure
```
.
├── index.html
├── README.md
└── public
    ├── css
    │   └── output.css
    ├── images
    │   ├── logo.webp
    │   ├── hero.image.webp
    │   ├── understanding.image.webp
    │   └── help.image.webp
    └── pages
        ├── about.html
        └── contact.html
```

## Design
| Role | Color |
| --- | --- |
| Accent / buttons | `#b95028` |
| Hero and card background | `#fce2d2` |
| Section background | `#f7ede5` |
| Text | `#6b6059` |
| White cards | `#ffffff` |

- **Section background (gradient):** `bg-linear-to-b from-[#fce2d2] to-[#f888]`
- Cards use `rounded-3xl` and `border-t-4`. Buttons use `rounded-full` and lift slightly on hover.
- Every page shares the same header and footer, and the active page is highlighted in the navbar.

## Typography

- **Font family:** [Space Grotesk](https://fonts.google.com/specimen/Space+Grotesk)

## Accessibility and safety

- Alt text on the hero images (about and contact pages), and decorative SVG icons are `aria-hidden`.
- Form: every field has a linked `label`, choices are grouped with `fieldset` and `legend`, and focus is visible.
- The form never asks for a real name or medical details, and every field is optional.
- No invented phone numbers, organisations or statistics. Anything that needs checking is marked with `[... VERIFY]`.

## Author
Samir Belgassab