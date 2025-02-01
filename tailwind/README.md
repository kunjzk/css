# Tailwind

Even better CSS experience than Bootstrap.

Methods of installation: https://tailwindcss.com/docs/installation/using-vite

- Easier use of classes (more like pseuocode)
- Nice Tailwind extension too on VSCode, but only works when you install tailwind CLI instead of running it in the "play" cdn mode.

## Installing Tailwind with NPM

Guide: https://tailwindcss.com/docs/installation/tailwind-cli

1. `npm init -y` to create a project (with package.json)
2. Follow the guide above. Imposes a certain structure on you.

- Generates an `output.css` file, massive file which defines a bunch of default classes and styling.
- Constantly watches your html file for changes. Tailwind extension now works in vscode, so you can start adding classes to the style of your html elements.
- Tailwind will monitor these changes, and define the appropriate classes in output.css (dynamically generated based on your changes to html) in the most efficient way.
- **_BASICALLY, tailwind automatically writes new CSS for you._**
- Need to learn the tailwind equivalent of traditional CSS. Eg: `justify-content: center` in the tailwind world is just the class `justify-center`: https://tailwindcss.com/docs/justify-content
