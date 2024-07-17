# search-engine-homepage

A recreation of a popular search engine's home page to demonstrate frontend proficiency.

## Dependency Notes

This project was created using [Node.js](https://nodejs.org/en) v20.11.0.

## Project Setup

When first checking out the repo or changing branches, run the following command in the terminal to ensure all packages are up to date:

```sh
npm install
```

### Compile and Hot-Reload for Development

To start the dev server, run the following command in the terminal:

```sh
npm run dev
```

You can then visit http://localhost:5173/ in your browser to interact with the site. Any changes you make will take effect without you having to refresh the page.

---

## Developer Remarks

This project recreates Google's home page as of 07/17/2024 as it appears to users in "dark mode". A snapshot of the page can be found in `./screenshots/reference.png`.

Examples of this project are stored in the `./screenshots/deliverable` folder and display the app in a variety of states and browser configurations.

The total time spent to create this project was roughly 6 hours and 45 minutes. If the project were to be given more time, areas of improvement include:

- Completing the functionality of the search field: Adding buttons for audio and image upload, implementing the expanded "history/tending" dialog. Clean up the search icon to better match the original (size and shape are slightly off).
- Extending the `UIButton` component to use the `animate` and `secondaryText` props to recreate the experience seen with the "I'm Feeling Lucky" button.
- Refactoring color references in the CSS into theme values and implementing a Light Mode style.
- Tweaking the styling of the footer: The leaf icon has a height that is different from the original which causes the footer to be slightly smaller and the alignment of the icon and text being slightly off.

---

## Languages and Tools

<p align="center">
  <a href="https://github.com/LelouchFR/skill-icons"><img src="https://go-skill-icons.vercel.app/api/icons?i=chrome" alt="Chrome" title="Chrome" /></a>
  <a href="https://github.com/LelouchFR/skill-icons"><img src="https://go-skill-icons.vercel.app/api/icons?i=css" alt="CSS" title="CSS" /></a>
  <a href="https://github.com/LelouchFR/skill-icons"><img src="https://go-skill-icons.vercel.app/api/icons?i=html" alt="HTML" title="HTML" /></a>
  <a href="https://github.com/LelouchFR/skill-icons"><img src="https://go-skill-icons.vercel.app/api/icons?i=javascript" alt="JavaScript" title="JavaScript" /></a>
  <a href="https://github.com/LelouchFR/skill-icons"><img src="https://go-skill-icons.vercel.app/api/icons?i=npm" alt="npm" title="npm" /></a>
  <a href="https://github.com/LelouchFR/skill-icons"><img src="https://go-skill-icons.vercel.app/api/icons?i=tailwindcss" alt="Tailwind CSS" title="Tailwind CSS" /></a>
  <a href="https://github.com/LelouchFR/skill-icons"><img src="https://go-skill-icons.vercel.app/api/icons?i=vite" alt="Vite" title="Vite" /></a>
  <a href="https://github.com/LelouchFR/skill-icons"><img src="https://go-skill-icons.vercel.app/api/icons?i=vscode" alt="VS Code" title="VS Code" /></a>
  <a href="https://github.com/LelouchFR/skill-icons"><img src="https://go-skill-icons.vercel.app/api/icons?i=vuejs" alt="Vue.js" title="Vue.js" /></a>
</p>
