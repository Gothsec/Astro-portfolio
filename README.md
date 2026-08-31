# Portfolio
> A minimal, highly customizable, and performant personal portfolio template built with Astro, React, and Tailwind CSS.

![OscarHernandez-portfolio](https://github.com/user-attachments/assets/e284a42b-15c5-495c-99c7-ad5c1eb3bbe7)
![Deploy Status](https://img.shields.io/badge/Deploy-Vercel-black?style=flat&logo=vercel)

---

[Demo](https://oscarhernandez.vercel.app/) | [Astro Themes](https://astro.build/themes/details/dark-minimal/) | [ReactBits Showcase](https://www.reactbits.dev/showcase) 

## **Features**
- 🚀 **Blazing fast performance** powered by Astro
- 🎨 **Beautifully styled** with Tailwind CSS
- 🎵 **Spotify integration** for showcasing your favorite album
- ✉️ **Working contact form** powered by Formspree
- ⚛️ **Interactive UI** including the `<LetterGlitch />` component from [ReactBits.dev](https://www.reactbits.dev/)

## **Stack**  
### **Frontend**  
![Astro](https://img.shields.io/badge/Astro-FF5D01?logo=astro&logoColor=white)
![Tailwind](https://img.shields.io/badge/Tailwind_CSS-38B2AC?logo=tailwind-css&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?logo=typescript&logoColor=white)

### **Tools**  
![Figma](https://img.shields.io/badge/Figma-F24E1E?logo=figma&logoColor=white)
![Prettier](https://img.shields.io/badge/Prettier-F7B93E?logo=prettier&logoColor=black)
![Canva](https://img.shields.io/badge/Canva-c900c3?logo=canva&logoColor=white)

## **Configuration Guides**

### **Show your favorite Spotify album (or your own)** ![Spotify](https://img.shields.io/badge/Spotify-06cc1a?logo=spotify&logoColor=white)
1. Choose your Spotify album
2. Access the share options
3. Select 'copy embed code'
```html
<iframe src="https://open.spotify.com/embed/album/YOUR_ALBUM_ID_HERE" style="border-radius:12px border:0;" class="w-full h-40" frameborder="0" allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture"></iframe>
```
4. Insert the embed code on `src/Components/footer.astro`

### **Set up contact form (Formspree)** ![Formspree](https://img.shields.io/badge/Formspree-E21A28?logo=formspree&logoColor=white)
1. Create an account on [Formspree](https://formspree.io/)
2. Create a new project/form and copy your form endpoint URL (it looks like `https://formspree.io/f/your_id`)
3. Open the `src/Components/contact.astro` file
4. Replace the `action` attribute in the `<form>` tag with your endpoint URL:
```html
<form action="https://formspree.io/f/YOUR_FORM_ID_HERE" method="POST">
```

## **Customization**
To make this portfolio your own, you can edit the following files:
- **Global Settings:** Update metadata and title in `src/layouts/Layout.astro`.
- **Content:** Modify the text, links, and details inside the components in `src/Components/` (e.g., `home.astro`, `projects.astro`, `contact.astro`).
- **Styling:** The design uses Tailwind CSS. You can adjust the theme configuration in `tailwind.config.mjs` and custom styles if needed.

## **Project structure**
```text
public/
└── svg/
src/
├── Components/
|    ├── contact.astro
|    ├── footer.astro
|    ├── home.astro
|    ├── logoWall.astro
|    ├── nav.astro
|    └── projects.astro
├── layouts/
|    └── Layout.astro
├── React/
|    ├── LetterGlitch.tsx
|    ├── LikeButton.tsx
|    └── SkillsList.tsx
└── pages/
     └── index.astro
```

## **Local configuration** 

### Prerequisites
- **Node.js** (v18 or higher recommended)
- **npm** or **pnpm**

1. Clone the repo:  
```bash
git clone https://github.com/Gothsec/Astro-portfolio
```
2. Install dependencies:
```bash  
npm install
```
3. Start the development server:
```bash  
npm run dev
```

## **Deployment**
This project is built with Astro and can be easily deployed to Vercel, Netlify, or GitHub Pages. For the easiest setup, push your repository to GitHub and import it directly into [Vercel](https://vercel.com/) or [Netlify](https://www.netlify.com/).

> **Important Notice:**  
> This project is licensed under the [MIT License](https://opensource.org/licenses/mit).  
> According to the license terms, any redistribution (including compiled or modified versions), you **must** retain the original copyright 
> notice and the full license text. Copyright © 2026 Oscar Hernandez. All rights reserved.
