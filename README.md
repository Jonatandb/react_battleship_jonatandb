# REACT DEVELOPMENT TEST

## Battleship game

### MAIN GOAL

Develop a simplified React version of the battleship game; player vs CPU.

### GAME ELEMENTS AND CHARACTERISTICS

- 10x10 board size
- 1 carrier of 4 spaces
- 3 cruisers of 3 spaces
- 1 submarine of 2 spaces
- Ships must be straight lines
- Ships can be placed horizontally or vertically

### BASIC GAMEPLAY

The game should have at least **3 screens** with the following components and actions.
<br/>All mockups are just for reference and can be improved.

#### START SCREEN

- Place your ships on the board
- Enter player name
- Button with “Start game” label

<p align="center">
    <img src="README_START_SCREEN.png" alt="Start Screen Screenshot"/>
</p>

#### GAME SCREEN

- Player and CPU boards
- Game state ("Playing: Player name or CPU")
- Clicking on computer board, you launch your missiles
- Launched missiles reference<br>HIT -orange-, DESTROYED -red-, MISSED/WATER -light blue-
- Attempt feedback (ship hit, ship destroyed, shot missed)
- CPU missiles can't be launched in random way (once the CPU hits a ship, the next shots must follow some strategy in order to sink the ship)
- Surrender button to end the game manually

<p align="center">
    <img src="README_GAME_SCREEN.png" alt="Game Screen Screenshot"/>
</p>

#### END GAME SCREEN

- Game result: won, lost, surrendered
- Restart button to go back to the Start screen

<p align="center">

```html
For more info about the game, check the Wikipedia article.
https://en.wikipedia.org/wiki/Battleship_(game)
```

</p>

### REQUIREMENTS

- You need to create a **GitHub repository** and send us the link so we can see the progress
- Please, try to **commit often and use clear and concise commit messages**
- The project must be **bootstrapped with Create React App** (<span>https</span>://github.com/facebook/create-react-app)
- Use **React Hooks** and avoid to use Classes
- You must use **Redux** to manage the application state
- Use **React Testing Library** to test the application
- Each component must have its **own test file**
- Tests all the features that you **consider to be relevant**
- Include **Snapshots Testing**
- Try to reach a **good percentage of coverage**
- Include **ESLint using Airbnb's ESLint Rules** (eslint-config-airbnb)
- Keep the use of **third-party packages to a minimum**
- Try to use the **latest versions of the packages** that are included
- **Add documentation**, highlight on complex logics
- Should work in the **latest versions of all major browsers** (Edge, Chrome, Firefox, Safari), both **desktop and mobile**
- Code and comments must be in **English**
- Keep in mind that we are going to analyze the code, look at **good practices, variable names, structures and so on, good luck!**

(_[PDF challenge file](<Battleship-FrontendReact(5).pdf>) by [Arzion](https://www.arzion.com/)_)

<p align="center">
    <img src="README_SHIPS.png" alt="Ships Screenshot"/>
</p>

---

### My Notes

#### Researched sites

- Markdown
  - [Mastering Markdown](https://guides.github.com/features/mastering-markdown)
  - [Markdown: Syntax](https://daringfireball.net/projects/markdown/syntax#html)
  - [Creating and highlighting code blocks](https://docs.github.com/en/github/writing-on-github/creating-and-highlighting-code-blocks)
  - [How do I prevent auto-generated links in the GitHub wiki?](https://stackoverflow.com/questions/25706012/how-do-i-prevent-auto-generated-links-in-the-github-wiki)
- Battleship Game
  - [Battleship (game)](<https://en.wikipedia.org/wiki/Battleship_(game)>)
  - [Batalla naval (juego)](<https://es.wikipedia.org/wiki/Batalla_naval_(juego)>)
- ESlint
  - [eslint-config-airbnb](https://www.npmjs.com/package/eslint-config-airbnb)
  - [Configuring ESLint](https://eslint.org/docs/user-guide/configuring)
  - [Prettier: ESLint Integrations](https://prettier.io/docs/en/related-projects.html#eslint-integrations)
  - [Extending Create React App's ESLint config](https://gaya.pizza/articles/extending-cra-eslint-airbnb/)
  - [Setting up Create React App, VS Code, ESLint, and Prettier](https://readwriteexercise.com/posts/setting-up-create-react-app-vs-code-eslint-prettier/)
  - [Airbnb Javascript style guide — Key takeaways](https://medium.com/docon/airbnb-javascript-style-guide-key-takeaways-ffd0370c053)
  - [Airbnb JavaScript Style Guide() {](https://github.com/airbnb/javascript)
  - [Create-react-app -> Setting Up Your Editor -> #Experimental: Extending the ESLint config](https://create-react-app.dev/docs/setting-up-your-editor/#experimental-extending-the-eslint-config)
  - [Qué es EsLint y por qué deberías usarlo](https://antoniomasia.com/que-es-eslint-y-por-que-deberias-usarlo/)
  - [React create-react-app v3.4.1 typescript: ESLint & Prettier with Airbnb style guides and VSCode WebStorm setup 2020](https://medium.com/react-courses/react-create-react-app-v3-4-1-a55f3e7a8d6d)
  - [VSCode + ESLint (AirBnb) + AutoFix on Save](https://www.youtube.com/watch?v=A0vyk3y4tDk)
  - [Improve Your Code With ESLint + VsCode + Airbnb Styleguide](https://www.youtube.com/watch?v=mfGkKlMDfwQ)
  - [VSCode ESLint, Prettier & Airbnb Style Guide Setup](https://www.youtube.com/watch?v=SydnKbGc7W8)
  - [VSCode - ESLint, Prettier & Airbnb Setup](https://gist.github.com/bradtraversy/aab26d1e8983d9f8d79be1a9ca894ab4)
  - [Integrating Prettier + ESLint + Airbnb Style Guide in VSCode](https://blog.echobind.com/integrating-prettier-eslint-airbnb-style-guide-in-vscode-47f07b5d7d6a)
  - [Configuring ESLint, Prettier and Airbnb in 1 Line](https://medium.com/javascript-in-plain-english/configuring-eslint-prettier-and-airbnb-in-1-line-164ab8f1e8c7) -[Can't get correct autoformat on save in Visual Studio Code with ESLint and Prettier](https://stackoverflow.com/questions/52102705/cant-get-correct-autoformat-on-save-in-visual-studio-code-with-eslint-and-prett)
  - [Conflict with react/jsx-one-expression-per-line #6456](https://github.com/prettier/prettier/issues/6456)
  - [eslint-config-react-app](https://github.com/facebook/create-react-app/tree/master/packages/eslint-config-react-app)
  - [eslint-config-prettier](https://github.com/prettier/eslint-config-prettier)
  - [eslint-plugin-prettier](https://github.com/prettier/eslint-plugin-prettier)
  - [eslint-plugin-react](https://github.com/yannickcr/eslint-plugin-react)
  - [Código limpio y consistente. ESLint + Prettier en tus proyectos con React.](https://dev.to/ericksarabia/codigo-limpio-y-consistente-eslint-prettier-en-tus-proyectos-con-react-462f)
