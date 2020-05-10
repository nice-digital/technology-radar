# Frontend

> **Adopt** - The default choice when selecting technologies
>
> **Assess**  - Technologies that we believe may be valuable, and are currently being assessed to understand their value and impact.
>
> **Hold** - Technologies in hold must no longer be used for new development

## Adopt
### React
Off-the-shelf tooling, popularity is insane, extremely engaged community, easy to recruit for. Used on External Consultations and Identity Management projects, as well as the Nice Design System.

### TypeScript
Microsoft's superset of JavaScript for static typing. TypeScript is "transcompiled" to JavaScript, showing errors at compilation. Used on Identity Management. The Design System supplies type definitions for TypeScript enabled projects.

### Jest + Enzyme
JS Testing framework. The default test driver for React when using Create-React-App. Enzyme is a testing utility that makes it easy to simulate interactions and assert on the output of React components. Used in consultations, IdAM, and the design system. Also the webdriver.io steps.

### Webpack
Module bundler for JavaScript (and other assets with plugins). Preferred approach to using JS on any new project or to be retrofitted where feasible.

### ES6 (or whatever is current)
We should be using modern syntax for JS wherever possible, as long as the code is transpiled before being used in the browser. Babel tooling makes adopting the latest spec recommendations very simple.

### Sass
CSS Preprocessor. Used on at least NICE Design System, Pathways and External Consultations.

### WebdriverIO
Front end testing framework. Used in everything. 

### Razor
Currently used in a few projects. For when you want .NET to render the HTML. We generally use React now, but sometimes we will use razor where react is overkill.

### npm
Currently standard, but can sometimes be a bit of a pain, so we are assessing yarn. 


## Assess
### Redux / Observable patterns / MobX / other state management
We're not currently using any state management approaches, would be good to assess for the next large single-page-app project.

### Gatsby / other static site generators
We have some sites that could do we being rewritten, and would be rewritten with a static site generators (eg CKS and BNF). Gatsby currently makes more sense than any other ones.

### Yarn
Trial to replace npm. **Do not** use both.

### Browserstack
cross browser testing

## Hold

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
For bundling, we use webpack

### Spark, Handlbars.js, nunjucks	
View engines, now out of date. We are using Razor or JSX templating

### Flow	
Trialled on comment collection, typescript does what flow does but better. Use typescript.

### Mocha
Used for previous versions of the design system, we use jest and enzyme instead.
