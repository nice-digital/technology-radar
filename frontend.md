# Frontend

> **Adopt** - The default choice when selecting technologies, currently in use in production
>
> **Assess**  - Technologies that we believe may be valuable, and are currently being assessed to understand their value and impact.
>
> **Hold** - Technologies in hold must no longer be used for new development

## Adopt

### React
Off-the-shelf tooling, popularity is insane, extremely engaged community, easy to recruit for. Used on External Consultations, Identity Management, CKS, BNF, Next Web, Global Nav, as well as the NICE Design System.

### TypeScript
Microsoft's superset of JavaScript for static typing. TypeScript is "transcompiled" to JavaScript, showing errors at compilation. Used on Identity Management and CKS. The Design System supplies type definitions for TypeScript enabled projects.

### ESNext
We should be using modern syntax for JS wherever possible, as long as the code is transpiled before being used in the browser. Babel tooling makes adopting the latest spec recommendations very simple. Although seriously consider [TypeScript](#typescript) over raw ESNext wherever possible.

### Jest
JS Testing framework. The default test driver for React when using Create-React-App and Gatsby etc. Used in most, if not all our 'modern' JavaScript projects.

### React Testing Library
React Testing Library replaces [Enzyme](#enzyme) as our library of choice for testing React components because of its [focus on user behaviour rather than internal implementations](https://testing-library.com/docs/react-testing-library/migrate-from-enzyme/#why-should-i-use-the-react-testing-library) of components, great docs and active community.

### Webpack
Module bundler for JavaScript (and other assets with plugins). Preferred approach to using JS on any new project or to be retrofitted where feasible. Used on CKS, via Gatsby, Global Nav, CKS, niceorg-client, NICE Design System, Comment Collection and probably others.

### Sass
CSS Preprocessor. Used almost everywhere (with modules) apart from a few legacy LESS projects here and there.

### WebdriverIO
Front end testing framework. Used in everything. 

### Razor
Currently used in a few projects. For when you want .NET to render the HTML. We generally use React now, but sometimes we will use razor where react is overkill.

### npm
Currently standard, but can sometimes be a bit of a pain. We decided to use this over yarn.

### NextJS
We see the need to have universal apps with Server Side Rendering (SSR) and whilst we're using React, NextJS makes sense. It provides SSR as well as static site generation (SSG) and even Incremental Static Regeneration (ISR) out of the box, has great docs, usage and community.

We used SpaServices in .NET Core 2 to provide server side React rendering, but this is out of support in August 2021. So we need an alternative for server-side rendered React apps, which may well be NextJS.

### Gatsby
CKS and BNF both use Gatsby. It provides a great developer experience, is performant, accessible and good for SEO. It has great documentation and large community. Usage of React and TypeScript in tandem with Jest and React Testing Library makes use of the Design System components seemless.


## Assess

### Redux / Observable patterns / MobX / other state management
We're not currently using any state management approaches, would be good to assess for the next large single-page-app project.

### Browserstack
Used for automated cross browser testing with WebdriverIO in at least 1 project.


## Hold

### Yarn
We see no reason to use yarn, especially with npm 7 out with Node 16+. People are comfortable with nvm tooling so there's no need to rock the boat with _another_ tool without clear reason. It _might_ be useful with the monorepo in the Design System (using workspaces), but Lerna plugs that gap.

### Enzyme
Enzyme was the de facto library for testing React components. However, React Testing Library is now more widely used (as of [September 2020](https://www.npmtrends.com/enzyme-vs-@testing-library/react)) and focuses more on behaviour than implementation so results in better tests.

### jQuery	
Now we're supporting IE11+, JavaScript in our target browsers is pretty aligned, or easier than ever to compensate for. 

If we are in control of the DOM, we use react. If not, eg content managed html, we don't.

### Cassette
Unmaintained asset bundler for .Net. Last update was in 2014.

### Meteor
Used by Medtech with MongoDB. Universal JavaScript app framework (runs same code on back and front end).

### Less
CSS pre-processor; lost the war with SASS. Used in at least Publications and Niceorg.

### Any bootstrap etc that isn't the NICE design system
Use the NICE design system

### Angular
We are using React

### Custom frameworks built on top of things eg hyperbone	
We are using React

### Backbone
We are using React

### Browserify/Grunt etc
For bundling, we use [webpack](#webpack)

### Spark, Handlbars.js, nunjucks
View engines, now out of date. We are using Razor or JSX templating

### Flow
Trialled on [Comment Collection](https://github.com/nice-digital/consultations), TypeScript does what Flow does but better and with better tooling. Use [TypeScript](#typescript).

### Mocha
Used for v0 of the Design System, we use Jest instead.
