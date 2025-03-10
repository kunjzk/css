# Tailwind

Even better CSS experience than Bootstrap.

Methods of installation: https://tailwindcss.com/docs/installation/using-vite

- Easier use of classes (more like pseuocode)
- Nice Tailwind extension too on VSCode, but only works when you install tailwind CLI instead of running it in the "play" cdn mode.

## Installing Tailwind with NPM

Guide: https://tailwindcss.com/docs/installation/tailwind-cli

1. `npm init -y` to create a project (with package.json)
2. Follow the guide above. Imposes a certain structure on you.
3. _ALWAYS RUN TAILWIND CLI_: `npx @tailwindcss/cli -i ./src/input.css -o ./src/output.css --watch`

## How it works + benefits

- Generates an `output.css` file, massive file which defines a bunch of default classes and styling.
- Constantly watches your html file for changes. Tailwind extension now works in vscode, so you can start adding classes to the style of your html elements.
- Tailwind will monitor these changes, and define the appropriate classes in output.css (dynamically generated based on your changes to html) in the most efficient way.
- **_BASICALLY, tailwind automatically writes new CSS for you._**
- Need to learn the tailwind equivalent of traditional CSS. Eg: `justify-content: center` in the tailwind world is just the class `justify-center`: https://tailwindcss.com/docs/justify-content
- Write CSS without leaving your HTML
- Reuse HTML components once styled: it'll always look the same in whatever project you use

## Responsive design

https://tailwindcss.com/docs/responsive-design

- Idea: target mobile first by prefixing your class with `sm` -- this is how your element behaves at and after the small breakpoint.

- Basic principle: mobile views tend to be row oriented, desktop tends to be columnar with 2 or 3 cols max and spacing around them. Once you go from desktop to mobile, all other colums disappear except 1 for the main content. `class="grid sm:grid-cols-4"`. By default, we want to have `hidden` and `sm:block` classes so that the element is hidden by default and toggled to display itself on larger screens. check example 3 in `layouts.html`.

- Larger displays tend to be divided into 12 sections. `col-span-n` property controls how many columns a div takes.
