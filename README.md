# react-dsmjs

## [React.render](https://facebook.github.io/react/docs/top-level-api.html#react.render)(ClientOrServer, document.querySelector(‘.you-decide’));

### It is the V in MVC
* Works well with other frameworks like Angular and Backbone
* JSX, combines your markup and behavioral JS
* Try to use primitive JS like arrays, objects and functions

### Virtual DOM
* Difs the real DOM, updates for you
* Removing and building DOM tree nodes is expensive

### One directional flow control
* Pass props down
* Only store state in Root component and pass a props to children

### Component Lifecycle
* [getInitialState](https://facebook.github.io/react/docs/component-specs.html#getinitialstate)
* [componentDidMount](https://facebook.github.io/react/docs/component-specs.html#mounting-componentdidmount)

### Rendering
* [render](https://facebook.github.io/react/docs/top-level-api.html#react.render) (client)
* [renderToString](https://facebook.github.io/react/docs/top-level-api.html#react.rendertostring) (server)
* [renderToStaticMarkup](https://facebook.github.io/react/docs/top-level-api.html#react.rendertostaticmarkup) (server)

Changes to state and props will cause component to render. I think this makes it easier to understand how and when a component is updated.

### Testing
* [ReactTestUtils](https://facebook.github.io/react/docs/test-utils.html)
* [JSDOM](https://github.com/tmpvar/jsdom)
* Allows you to test drive behavioral styles like display
* [Chrome Dev Tools Extension](https://chrome.google.com/webstore/detail/react-developer-tools/fmkadmapgofadopljbjfkapdkoienihi?hl=en)
* [React TDD Guide](https://github.com/zpratt/react-tdd-guide)

### Usage

Before using React we were using a mixture of Backbone and Mustache. This was harder to understand the interaction between the view and the template, and context switching between two files. We currently use Webpack to compile JSX with Babel and SCSS. We require in our `.scss` files with components so they can be lazily loaded and better namespaced.

We are currently working on newer NodeJS based applications where React is used on both sides of the stack. Being able to write once and choose where to render is great. We are able to truly AB test what is most performant.

### React Native
I haven't spent any time trying to develop anything with it yet, but seems interesting
