# react-dsmjs

## React.render(ClientOrServer, document.querySelector(‘.you-decide’));

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
* getInitialState
* setState
* componentDidMount

### Rendering
* render (client)
* renderToString (server)
* renderToStaticMarkup (server)

Changes to state and props will cause component to render. I think this makes it easier to understand how and when a component is updated.

### Testing
* ReactTestUtils
* JSDOM
* Allows you to test drive behavioral styles like display
* Chrome Dev Tools Extension
* Zachs testing React project
* 

### Usage

Before using React we were using a mixture of Backbone and Mustache. This was harder to understand the interaction between the view and the template, and context switching between two files. We currently use Webpack to compile JSX with Babel and SCSS. We require in our `.scss` files with components so they can be lazily loaded and better namespaced.

We are currently working on newer NodeJS based applications where React is used on both sides of the stack. Being able to write once and choose where to render is great. We are able to truly AB test what is most performant.

### React Native
I haven't spent any time trying to develop anything with it yet, but seems interesting
