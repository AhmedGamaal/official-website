# Energia Powered Official Webite

This's the main source code of the front of `Energia Powered` website.

## The structure of the website

- assets - here are all the images or any assets we may need
- components - here are all presentational components that has no business logic
  - ExampleComponent (e.g: Footer)
    - index.js
    - style.css
    - tests
- containers - here are all components that has business logic
  - ExampleComponent
    - index.js
    - style.css
    - tests
- pages - here are all the components that represents the react routes
  - HomePage
    - index.js
    - index.css
    - components
      - Header
        - index.js
        - style.css
        - tests
    - tests

**Tools used**

1. [Fontawesome](https://scotch.io/tutorials/using-font-awesome-5-with-react) - [Footer Component Demo](https://github.com/EnergiaPowered/official-website/blob/master/front/src/components/HomePage/Footer.js)

2. [React-multi-carousel](https://www.npmjs.com/package/react-multi-carousel) - [Partners Component Demo](https://github.com/EnergiaPowered/official-website/blob/master/front/src/components/HomePage/Partners/Partners.js)

3. [Bootstrap 4.3](https://getbootstrap.com/)

4. [react-testing-library](https://github.com/testing-library/react-testing-library)

5. [Jest](https://jestjs.io/docs/en/getting-started)

**Notes:**

- Routing is already setup - Go to `front/src/App.js` file and add your routes
- Add the Homepage Sections at `front/src/pages/HomePage/index.js`

**Tips:**

- To set the background image of the header properly:

  - First, we should look on the example structure

```
HomePage (The container component)
- HomePage
    - index.js
    - index.css
    - components
    - Header
        - index.js
        - style.css
        - tests
    - tests

```

  1. Make the container component and give it `page-component` class like that in [`front/src/pages/HomePage/index.js`](https://github.com/EnergiaPowered/official-website/blob/master/front/src/pages/HomePage/index.js) and give it the appropriate background image like that in [`front/src/pages/HomePage/index.css`](https://github.com/EnergiaPowered/official-website/blob/master/front/src/pages/HomePage/index.css)

  2. Make the header component and give it `header-section` class like that in [`front/src/pages/HomePage/Header/index.js`](https://github.com/EnergiaPowered/official-website/blob/master/front/src/pages/HomePage/Header/index.js)

  3. Make the sub header component and give it the class `bg-section` like that in [`front/src/pages/HomePage/Supervisor/index.js`](https://github.com/EnergiaPowered/official-website/blob/master/front/src/pages/HomePage/Supervisor/index.js)
  4. Make the other components and give it `bg-section` and control the spaces as u like

- To set the font size of each component properly:

  1. Every main section should have the structure:

     - The title of the section should be `h2` tag with the classes `section-title text-center`
     - The rest of the content

  2. Give the root tag in the component the class `component-font` like that in [`front/src/pages/HomePage/Supervisor/index.js`](https://github.com/EnergiaPowered/official-website/blob/master/front/src/pages/HomePage/Supervisor/index.js)