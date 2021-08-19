# GSoC-2021-Project-Report
Final report for Google Summer of Code - 2021 at Python Software Foundation (EOS)
## EOS-Icons npm Package for React and Vue
![EOS_ICONS_03056bacea](https://user-images.githubusercontent.com/54861487/129490915-26b618e4-6cf5-415d-952e-76c83f181bbc.png)

## Project Summary
Currently EOS delivers icons via a set of well documented methods, which chiefly include EOS-Icons Package, CDN or direct download of icons in SVG/PNG formats. The goal of this project was to develop an npm package that can deliver EOS Icons to its users as an independent component library and create a unified central system that will enable EOS to deliver its icons to various frameworks (e.g. React, Vue and Angular) independently. The EOS-Icons React npm package, Vue 3 npm package as well as Vue 2 npm package (under-development) are as lightweight as possible in order to reduce the load put on the browser (using the tree shaking approach). The React npm package and Vue 3 npm package supports both TypeScript as well as JavaScript based projects. The Icon component provides the user with multiple props like Size, color, rotation, theme and flip (horizontal, vertical).

## Development process
![126060393-13098cd1-e7aa-4fb7-8634-b15e3369f7ff](https://user-images.githubusercontent.com/54861487/129492131-9bacd2b2-8b74-4f28-a2bd-ac0eab78d228.png)

## Contributions
### React
- Used Gulp for automating the task of fetching the new SVG files from EOS-ICONS as well as clearing out the build folder
- Created a script for scaffolding SVG icons into React components
- Build process for outputing the React components into esnext and commonjs format for supporting JS and TS
- Props for Size, Color, Rotation, Flip and theme (common components)
- Testing the final built components using Jest
- Configured semantic release for the repo based on eslint conventions
- Custom class support for providing external css
- Function for converting PascalCase into SCREAMING_SNAKE_CASE
- Config for changing the default props of the package
- Script for scaffolding React components into Storybook stories (website - https://storybook.eos-icons.com)
### Vue (2/3)
- Testing Vue Functional components using Jest (Vue 3)
- Structure for supporting treeshaking (based on EOS-Icons React npm package, mentioned above)
- Vue-styled components for supporting Vue 2 based projects (Vue 2)
- Implementation of Rollup for building TypeScript Vue components into commonjs and esnext format
## More info about the project:
React - [My Code contributions](https://github.com/EOS-uiux-Solutions/eos-icons-react/pulls?q=is%3Apr+is%3Aclosed+author%3Avinayaksh42), [Project Readme](https://github.com/EOS-uiux-Solutions/eos-icons-react/blob/main/README.md), [npm link - EOS-Icons React](https://www.npmjs.com/package/eos-icons-react)

Vue 3 - [My Code contributions](https://github.com/EOS-uiux-Solutions/eos-icons-vue/pulls?q=is%3Apr+is%3Aclosed+author%3Avinayaksh42), [Project Readme](https://github.com/EOS-uiux-Solutions/eos-icons-vue/blob/main/README.md), [npm link - EOS-Icons Vue3](https://www.npmjs.com/package/eos-icons-vue3)

Vue 2 - [My Code contributions](https://github.com/EOS-uiux-Solutions/eos-icons-vue2/pulls), [Project Readme](https://github.com/EOS-uiux-Solutions/eos-icons-vue2/blob/main/README.md), [npm link - EOS-Icons Vue2](https://www.npmjs.com/package/eos-icons-vue2)

## My journey
I have written blogs about my GSoC work - [GSoC PSF blogs](https://blogs.python-gsoc.org/en/vinayaksh42s-blog/)

## Future Ideas
- Developing a npm package for Angular framework and React native (highly being used for app development)
- Adding more props like [skew](https://developer.mozilla.org/en-US/docs/Web/SVG/Attribute/transform#skewx)
- More tests for checking component attributes after applying multiple props
- Creating a component in which the user can pass SVG and utilise the prop customization provided by eos-icons
- Adding a new section to [EOS Icons website - docs](https://eos-icons.com/docs) for guiding the user with installation and usage process.

## Thank you
The past few months have been no less than magical! I had a lot of fun and learned a lot over this time duration all because of the endless support of my awesome mentors. Google Summer of Code with the EOS community was by far the best experience. The guidance provided for setting up my development enviroment in a more proficient way to helping me solve complicated problems will surely help me in becoming a better developer. Will keep on contributing to EOS 💖
