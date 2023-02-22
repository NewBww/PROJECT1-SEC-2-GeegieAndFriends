# Project Music Player (Release v2.0.0)

##### By _Geegie and Friends_, an INT203 Project Team

A Vue music player project for INT203 Class created for education purposes only.

Open and view the Project using the `.zip` file provided or at my [GitHub Repository]

The project is also hosted on [Netlify](https://geegie.netlify.app) (for development preview using this [link](https://geegie-dev.netlify.app))

## Table of Contents

- [Getting Started](#getting-started)
  - [Tools Required](#tools-required)
  - [Installation](#installation)
- [Development](#development)
  - [Sprint 1: Planning and Project Setup](#sprint-1-planning-and-project-setup)
    - [Step 1: Project and repository preparation](#step-1-project-and-repository-preparation)
    - [Step 2: Work flow planning and choosing the topic](#step-2-work-flow-planning-and-choosing-the-topic)
  - [Sprint 2: Home page UI and Music Player](#sprint-2-home-page-ui-and-music-player)
    - [Step 1: Design the homepage for the application](#step-1-design-the-homepage-for-the-application)
    - [Step 2: Coding the music player component and layout for the homepage](#step-2-coding-the-music-player-component-and-layout-for-the-homepage)
  - [Sprint 3: Main Function for Homepage](#sprint-3-main-function-for-homepage)
    - [Step 1: Refactor the code from previous sprint](#step-1-refactor-the-code-from-previous-sprint)
    - [Step 2: Planning the backlog for this sprint](#step-2-planning-the-backlog-for-this-sprint)
    - [Step 3: Develop new features for the app](#step-3-develop-new-features-for-the-app)
- [Running the App](#running-the-app)
- [Deployment](#deployment)
- [Versioning](#versioning)
- [Contributors](#contributors)
- [Authors](#authors)
- [Acknowledgments](#acknowledgments)

## Getting Started

The two primary branches in the project are `main` and `dev`.

- `main` contains the production version of the application code
- `dev` contains code under development

The project structure:

```
    PROJECT1-SEC-2-GeegieAndFriends
	├── README.md
	├── package.json
	├── .gitignore
	├── .stylelintrc.json
	├── .yarnrc.yml
	├── .gitignore
	├── package.json
	├── postcss.config.js
	├── tailwind.config.js
	├── vite.config.js
	├── yarn.lock
	├── index.html
	├── .github
	│   └── workflows
	│       └── unit-test.yml
	├── .yarn
	│   ├── cache
	│   └── releases
	├── public
	│   ├── favicon.ico
	│   └── tracks
	└── src
	    ├── assets
	    │   ├── img
	    │   └── main.css
	    ├── App.vue
	    └── Main.js
```

### Tools Required

You would require the following tools to develop and run the project:

- A text editor or an IDE (Recommended: _WebStorm_ or _Visual Studio Code_)
- _NodeJs_ v16.9.0 or later
- _Yarn_ for package management

### Installation

These installation steps are required to build the project from your local machine.

- Install NodeJs from this [_link_](https://nodejs.org/en/download/)
- Install Yarn through the [_npm package manager_](http://npmjs.org/):

  ```
  npm install --global yarn
  ```

  Check the version of Yarn by running:

  ```
  yarn --version
  ```

## Development

This section includes the development strategies, processes and contributions within the project.

### Sprint 1 Planning and Project Setup

#### Step 1 Project and repository preparation

- Create a new project with the IDE.
  - Integrating Yarn, Tailwind, etc.
  - Refactoring a package.json file.
- Setup [Netlify] for the project.
  ![The Netlify site overview for the production branch](img/netlify-site-overview.png 'Site Overview')
- Putting additional tools in the tech stack.
  - PostCSS: a transpiler that turns a special PostCSS plugin syntax into a Vanilla CSS
  - Autoprefixer: a plugin to parse CSS and add vendor prefixes to CSS rules using values from _Can I Use_.
  - Stylelint: a linter for set the CSS style rules.

#### Step 2 Work flow planning and choosing the topic

- Brainstorm the topic we want to practice and working on
- Chose a topic of music player app from 3 ideas including the split share app and restaurant recommendation app
  ![Top 3 topic we picked from the brainstorm session](img/topic-ideas.png 'Topic Ideas')
- Discussing how to contribute within the team.
  - Created the GitHub project for managing the task for contributors to pick their task.
    ![A todo board for organizing task within the team](img/github-projects-board.png 'Todo Board')
- Setup GitHub workflow for the future unit tests and linters optionally.
  ![Create unit test workflow for GitHub Actions](img/unit-test-workflow.png 'Unit Tests Workflow')

  For details now how everything has been implemented, refer the source code

### Sprint 2 Home page UI and Music Player

#### Step 1 Design the homepage for the application

- Finding some references for inspiration
- Drafting the homepage and some other pages for the future
  ![The first draft was paticipated by every contributors](img/first-draft.png 'The First Draft')
- Develop the design system for the whole project
  ![a music player component for reuse in the design](img/design-sys-music-player.png 'Music Player Component Design')
  ![Collection of color to use in the design](img/theme-and-colors.png 'Theme and Colors')
- Redesign in Figma
  ![Final design of the release v1.0.0](img/homepage-final.png 'The Redesigned Homepage')

#### Step 2 Coding the music player component and layout for the homepage

- Developing the music player algorithm in `dev` branch
  ![Some preview for the Vue source code](img/code-preview.png 'Code Preview')
- Layout for the homepage in `template` branch

### Sprint 3 Main Function for Homepage

#### Step 1 Refactor the code from previous sprint

- Changing to composition API
- Optimize the code, reduce redundancy, grouping the utility functions

#### Step 2 Planning the backlog for this sprint

![Feature in progress during sprint 3](img/sprint-3-backlog.png "Sprint 3 Todo list")

#### Step 3 Develop new features for the app

![Home page with many new features](img/sprint-3-final.png "Final Release of sprint 3")
- includes
  - carousel playlist
  - queuing system
  - shuffle song
  - drag-to-seek progress bar
  - choose and play music from trending list

## Running the App

Steps and commands for running the app:

### Compile and Hot-Reload for Development

```sh
yarn dev
```

### Compile and Minify for Production

```sh
yarn build
```

### Preview for Production

```sh
yarn preview
```

## Deployment

The `main` branch is automatically deployed to production on [geegie.netlify.app]

The `dev` branch is automatically deployed to preview the development on [geegie-dev.netlify.app]

This documentation also hosted on [Github Pages]

## Versioning

```
  Pre-release v1.0.0
  ----------------------------------------------------------------------------------
  [New] Music Player Component
  [New] Homepage
  ----------------------------------------------------------------------------------
```

## Contributors

| Student ID  | Name                     | Email                      | Github Username |
|-------------|--------------------------|----------------------------|-----------------|
| 64130500066 | Phutawan Palakavong      | Phutawan.pala@kmutt.ac.th  | [pphtw]         |
| 64130500079 | Siripoom Kusonsong       | Siripoom.kuso@kmutt.ac.th  | [PhuMiZz]       |
| 64130500080 | Supapit Krawsaikom       | Supapit.kraw@kmutt.ac.th   | [supapitploy]   |
| 64130500105 | Banlearit Siriboon       | Banlearit.siri@kmutt.ac.th | [Banlearit]     |
| 64130500119 | Bowonwit Anothaisintavee | Bowonwit.anot@kmutt.ac.th  | [NewBww]        |

You can also see the complete [list of contributors][Contributors] who participated in this project.

## Authors

#### _Bowonwit Anothaisintavee_

- [Github](https://github.com/NewBww)

## Acknowledgments

This section can also be called as `Resources` or `References`

### Credits

Music in this project

- [Matsuri](https://youtu.be/NwOvu-j_WjY) (Song by _Fujii Kaze_) Licensed to YouTube by UMG (on behalf of Universal Music LLC); UMPG Publishing, BMI - Broadcast Music Inc., NexTone Inc. (Publishing), and 5 Music Rights Societies
- [double take](https://youtu.be/R8FHtIhWqNo) (Song by _dhruv_) Licensed to YouTube by SME (on behalf of Little Worry/RCA Records); BMI - Broadcast Music Inc., LatinAutor, LatinAutorPerf, and 11 Music Rights Societies
- [วาดไว้ (recall)](https://youtu.be/a0M_QUS3kC0) (Song by _BOWKYLION_) Licensed to What The Duck
- [After Rain (Scarlet Version)](https://youtu.be/BLqH4O7zq0s) (Song by _Aimer_) Provided to YouTube by Sony Music Labels Inc.
- [Attention](https://youtu.be/kdOS94IjzzE) (Song by _NewJeans_) Provided to YouTube by 'ADOR'
- [Cookie](https://youtu.be/0M4QMVQJRsw) (Song by _NewJeans_) Provided to YouTube by 'ADOR'
- [Ditto](https://youtu.be/-g9I2neQR7w) (Song by _NewJeans_) Provided to YouTube by 'ADOR'
- [Hurt](https://youtu.be/8QWtOgBJZNc) (Song by _NewJeans_) Provided to YouTube by 'ADOR'
- [Hype Boy](https://youtu.be/ghrlZIMDzbM) (Song by _NewJeans_) Provided to YouTube by 'ADOR'
- [夜に駆ける (Racing into the Night)](https://youtu.be/by4SYYWlhEs) (Song by _Yoasobi_) Provided to YouTube by The Orchard Enterprises
- [OMG](https://youtu.be/2Kff0U8w-aU) (Song by _NewJeans_) Provided to YouTube by 'ADOR'
- [Orion](https://youtu.be/lzAyrgSqeeE) (Song by _Kenshi Yonezu_) Provided to YouTube by Sony Music Labels Inc.
- [Overdose](https://youtu.be/H08YWE4CIFQ) (Song by _natori_) Provided to YouTube by The Orchard Music (on behalf of なとり) 
- [Pretender](https://youtu.be/37W7Y2RRyiM) (Song by _Official髭男dism_) Provided to YouTube by ポニーキャニオン
- [好きだから。](https://youtu.be/jlZJcx2Ighc) (Song by _Yuika_) Provided to YouTube by Universal Music Group
- [Zenzenzense](https://youtu.be/Mw66DyjQxBI) (Song by _RADWIMPS_) Provided to YouTube by TuneCore Japan
- [2002](https://youtu.be/1tvLIhEaEKo) (Song by _Anne-Marie_) 
- [About Time](https://youtu.be/ACFSpkO-b48) (Song by _Dept_) Provided to YouTube by WM Korea
- [Christmas Tree](https://youtu.be/1oq8Iesr1AU) (Song by _V_) Provided to YouTube by NHN BUGS
- [Daisy](https://youtu.be/NutHKRKBgR0) (Song by _Katy Perry_) Provided to YouTube by 2020 Capitol Records, LLC
- [Far Away](https://youtu.be/40uhlWGibBA) (Song by _Peter Fenn_) Provided to YouTube by DMRS Ltd
- [Favorite Thing](https://youtu.be/8Yx7-gGd6JI) (Song by _Rangga Jones_) Provided to YouTube by Believe SAS
- [Forever Rain](https://www.youtube.com/watch?v=Cvb76hBX_Oc) (Song by _RM_) Provided to YouTube BigHit Entertainment
- [Love Song](https://youtu.be/X03kXXiQHaQ) (Song by _Dept_) Provided to YouTube by WM Korea
- [Magic Shop](https://youtu.be/38k5zr1e0HI) (Song by _BTS_) Provided to YouTube by Big Hit Ent.
- [Stay](https://youtu.be/evBAiaYal1o) (Song by _BTS_) Provided to YouTube by Big Hit Ent.
- [Wave](https://youtu.be/JCLPMoT8FRY) (Song by _Fiji Blue_) 
- [ทรงอย่างแบด (Bad Boy)](https://youtu.be/cqQAzpZBpAw) (Song by _Paper Planes_) 
- [Guitar, Loneliness and Blue Planet](https://youtu.be/SDk1RA4g8CA) (Song by _Kessoku Band_) Provided to YouTube by Aniplex Inc.
- [Timemachine](https://youtu.be/oMwm_Km9YhU) (Song by _ปอน นิพนธ์ x โต๋ เหน่อ_)
- [I Like You (A Happier Song)](https://youtu.be/7aekxC_monc) (Song by _Post Malone_)
- [Night Dancer](https://youtu.be/QbHBfxAOucI) (Song by _imase_)
- [Say It](https://youtu.be/F64yFFnZfkI) (Song by _Yorushika_)
- [Stay](https://youtu.be/kTJczUoc26U) (Song by _The Kid Laroi_)
- [Blinding Lights](https://youtu.be/fHI8X4OXluQ) (Song by _The Weeknd_) 
- [Comedy](https://youtu.be/sKWYqop8pOc) (Song by _Miori Celesta_) Provided to YouTube by DistroKid
- [踊り子](https://youtu.be/7HgJIAUtICU) (Song by _Vaundy_)
- [YOU AND I](https://youtu.be/pH-rL_7TuTA) (Song by _Music oc | Missizfreak_)
- [Dandelions](https://youtu.be/W8a4sUabCUo) (Song by _Ruth B._)
- [Everything Goes On](https://youtu.be/izHyKdrSKvo) (Song by _Porter Robinson_) 
- [Wish You Were Sober](https://youtu.be/hEDBZtmKPmg) (Song by _Conan Gray_) Official music video by Conan Gray performing "Wish You Were Sober"
- [See You Again](https://youtu.be/RgKAFK5djSk) (Song by _Wiz Khalifa feat. Charlie Puth_)
- [Perfect](https://youtu.be/2Vv-BfVoq4g) (Song by _One Direction_) 
- [Die For You](https://youtu.be/QLCpqdqeoII) (Song by _The weeknd_) Provided to YouTube by Universal Music Group
- [Pano](https://youtu.be/s3eKZJI-oKA) (Song by _Zack Tabudlo_)
- [Heres Your Perfect](https://youtu.be/cRi-x2r88no) (Song by _Jamie Miller_) 
- [Dive Into You](https://youtu.be/hlrP9GXTx84) (Song by _NCT DREAM_) Provided to YouTube by SM Entertainment
- [Cant slow me down](https://youtu.be/xU2U73Tk-DM) (Song by _Mirani, lIlBOI, GroovyRoom, VALORANT_)
- [idontwannabeyouanymore](https://youtu.be/-tn2S3kJlyU) (Song by _Billie Eilish_)
- [17 นาที](https://youtu.be/qDrMDFhTdTw) (Song by _MILLI ft. mints (Prod. by SpatChies) | YUPP!_) 
- [Damn Good Day](https://youtu.be/PUJ9qXbLyfE) (Song by _Hoshimachi Suisei_) Provided to YouTube by cover corp.

### Inspirations

- [Music Player Web App](https://dribbble.com/shots/18946599-Music-Player-Web-App) (Dribble)
- [Web Music Player Concept](https://dribbble.com/shots/19753283-Web-Music-Player-Concept) (Dribble)

[//]: # 'HyperLinks'
[GitHub Repository]: https://github.com/NewBww/PROJECT1-SEC-2-GeegieAndFriends
[GitHub Pages]: https://NewBww.github.io/PROJECT1-SEC-2-GeegieAndFriends
[Contributors]: https://github.com/NewBww/PROJECT1-SEC-2-GeegieAndFriends/graphs/contributors
[Netlify]: https://geegie.netlify.app
[geegie.netlify.app]: https://geegie.netlify.app
[geegie-dev.netlify.app]: https://geegie.netlify.app
[//]: # 'Contributors Links'
[pphtw]: https://github.com/pphtw
[PhuMiZz]: https://github.com/PhuMiZz
[supapitploy]: https://github.com/supapitploy
[Banlearit]: https://github.com/Banlearit
[NewBww]: https://github.com/NewBww