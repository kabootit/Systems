# How I Do Stuff

- [Approach](#approach)
- [Design](#design)
- [Functional Programming](#functional-programming)
- [Cycle.js](#cyclejs)
- [Components](#components)
- [GraphQL](#graphql)
- [Tools](#tools)
- [Typescript](#typescript)
- [React Native](#react-native)
- [Server](#server)
- [Docker](#docker)
- [Git](#git)
- [Build](#build)
- [Testing](#testing)
- [Error handling](#error-handling)
- [Deployment](#deployment)
- [Websites](#websites)
- [Performance](#performance)
- [Progressive](#progressive)
- [Management](#management)
- [Business](#business)


## Approach

1. Surface area: Big is harder to control. Effort goes a lot further (efficient) if surface area smaller.
2. Taco Bell approach: use same 8 ingredients for everything.
3. Cognitive load: it's real. [Wiki](https://en.wikipedia.org/wiki/Cognitive_load) | [Reducing Cognitive Load](https://blog.marvelapp.com/design-principles-reducing-cognitive-load/)
4. [You are not being paid to code!](http://bravenewgeek.com/you-are-not-paid-to-write-code/)
5. [Why Deadlines Need to Drop Dead](https://medium.com/javascript-scene/why-deadlines-need-to-drop-dead-321739ae6be1#.43nmmmhp7)
6. [Mental models](https://medium.com/@yegg/mental-models-i-find-repeatedly-useful-936f1cc405d#.6frdlkfyb)

## Design

- [The design and implementation of software systems](http://zsck.co/2016/03/31/the-design-and-implementation-of-software-systems/)
- [NoSQL data modeling techniques](https://highlyscalable.wordpress.com/2012/03/01/nosql-data-modeling-techniques/)

## Functional Programming

- [What is a Closure?](https://medium.com/javascript-scene/master-the-javascript-interview-what-is-a-closure-b2f0d2152b36#.w1dsbzj5c)
- [Making Your JavaScript More Functional](https://adam.merrifield.ca/2016/11/01/making-your-javascript-more-functional/)
- [What makes functional programming so viable for problem modeling?](https://github.com/staltz/ama/issues/4)
- [The Reactive Extensions for JavaScript](https://github.com/Reactive-Extensions/RxJS)
- [10 Need-to-Know RxJS Functions with Examples](https://www.sitepoint.com/rxjs-functions-with-examples/)
- [Handle Branching Logic with Ramda's Conditional Functions](https://egghead.io/lessons/javascript-handle-branching-logic-with-ramda-s-conditional-functions)


## cyclejs

- [Gitter](https://gitter.im/cyclejs/cyclejs)
- [sharing data across application not in a parent-child component hierarchy](https://github.com/staltz/cycle-onionify/issues/3#issuecomment-254655941)
- [Refactor your cycle (app) into replaceable, reusable spare parts](https://journal.artfuldev.com/stop-breaking-your-head-refactor-your-cycle-app-into-replaceable-reusable-spare-parts-now-e10affed4e7d#.j2cnyxdwk)
- [Structuring Larger Applications](https://github.com/cyclejs/cyclejs/wiki/Structuring-Larger-Applications-(Guidelines))
- [Creating a Scalable JavaScript Application with Cycle.js](https://medium.com/@domagojk/creating-a-scalable-javascript-application-with-cycle-js-589f4d4020a5#.yjfpotio0) ([cycle-grid-driver](https://github.com/domagojk/cycle-grid-driver))
- [culli: manage your application state](https://github.com/milankinen/culli)
- [Redux DevTools extension](https://github.com/zalmoxisus/redux-devtools-extension)

## Components

1. Components with cyclejs

> Personally I've just been using styling from Bootstrap (via the LESS source, haven't used any of the JS stuff) and have found it works pretty well with CSS Modules when you just @import the parts of Bootstrap you actually need and compose what you need from it into your component's classes. PureCSS should be far more CSS Modules friendly since a lot of the styles are more compartmentalized

### Examples

- https://github.com/Bertrand31/Monitaure
- https://monitaure.io/tour
- http://quasar-framework.org/guide/

### Techniques

- https://github.com/erikras/styled-components
- https://github.com/erikras/styled-components-theme




## GraphQL

- [Super simple GraphQL server with Hapi.js, MongoDB and a new Apollo Server](https://blog.callstack.io/super-simple-graphql-server-with-hapi-js-mongodb-and-a-new-apollo-server-41418ded2faf#.ym09exd3c)
- [Join Monster: GraphQL-to-SQL query execution](https://www.npmjs.com/package/join-monster)
- http://graphql.org/code/
- https://www.npmjs.com/package/apollo-server
- https://www.reindex.io/blog/building-a-graphql-server-with-node-js-and-sql/
- https://blog.risingstack.com/graphql-overview-getting-started-with-graphql-and-nodejs/
- https://github.com/RisingStack/graphql-server
- https://dev-blog.apollodata.com/graphql-subscriptions-in-apollo-client-9a2457f015fb#.c7h7vssrd
- [5 benefits of static GraphQL queries](https://dev-blog.apollodata.com/5-benefits-of-static-graphql-queries-b7fa90b0b69a#.5544984rp)
- [Realtime GraphQL](https://dev-blog.apollodata.com/graphql-subscriptions-in-apollo-client-9a2457f015fb#.iwixrdc9n)
- https://github.com/OlegIlyenko/graphiql-workspace

## Tools

- [Secure tunnels to localhost](https://ngrok.com/)

## Typescript

## React Native

- http://www.reactnativeexpress.com/
- [Exponent: Rails for React Native](https://www.getexponent.com/)
- https://hashnode.com/post/what-we-learned-after-using-react-native-for-a-year-civdr8zv6058l3853wqud7hqp

### Starting point

- [Nativebase](http://nativebase.io/)
- [React Templates](https://wix.github.io/react-templates/)
- [Egghead Course](https://egghead.io/courses/react-native-fundamentals)


## Server

- [Introduction to Node & Express](https://medium.com/javascript-scene/introduction-to-node-express-90c431f9e6fd#.y46j1oo7t)

## Docker

- [8 protips](https://nodesource.com/blog/8-protips-to-start-killing-it-when-dockerizing-node-js/)
- [Manage Data within Docker Volumes](https://egghead.io/lessons/tools-manage-data-within-docker-volumes)


## Git

- [giteveryday(7) Manual Page](https://www.kernel.org/pub/software/scm/git/docs/giteveryday.html)
- [Git from the inside out](https://codewords.recurse.com/issues/two/git-from-the-inside-out)
- [Course: Practical Git](https://egghead.io/courses/practical-git-for-everyday-professional-use)
- [Mono repo](https://github.com/lerna/lerna) ([New wave modularity with Lerna, monorepos, and npm organizations](http://www.macwright.org/2016/07/08/lerna-npm-organizations-new-wave-modularity.html))

## Build

- [Webpack — The Confusing Parts](https://medium.com/@rajaraodv/webpack-the-confusing-parts-58712f8fcad9#.y9xum0f3s)
- [Getting Started with Webpack 2](https://blog.madewithenvy.com/getting-started-with-webpack-2-ed2b86c68783#.bbrn9ppa4)
- [Getting started with Webpack, part 2](https://blog.madewithenvy.com/getting-started-with-webpack-2-ed2b86c68783#.1ucztos07)


## Testing

- https://remysharp.com/2015/12/14/my-node-test-strategy
- https://remysharp.com/2016/02/08/testing-tape-vs-tap
- [5 Common Misconceptions About TDD & Unit Tests](https://medium.com/javascript-scene/5-common-misconceptions-about-tdd-unit-tests-863d5beb3ce9#.j4omeb29u)
- [Migrating Ava to Jest](http://browniefed.com/blog/migrating-ava-to-jest/)
- [Migrating to Jest](https://medium.com/@kentcdodds/migrating-to-jest-881f75366e7e#.l3uxfuorq)
- [Course: Testing JavaScript with Jest](https://egghead.io/playlists/testing-javascript-with-jest-a36c4074)
- [React Jest Workshop](https://github.com/kentcdodds/react-jest-workshop)

## Error handling

- https://www.joyent.com/node-js/production/design/errors

## Websites

- [Prose: Edit Github](http://prose.io/#kabootit)
- [Put yourself on internet with Jekyll, GitHub and Cloudflare](http://adgllorente.com/2016/09/put-yourself-on-internet-with-jekyll-github-and-cloudflare/)([HN](https://news.ycombinator.com/item?id=12558718))


## Deployment

- [Deploy secrets](https://egghead.io/lessons/node-js-use-secrets-when-deploying-applications-with-now)
- [Secret Management with Vault](http://chairnerd.seatgeek.com/secret-management-with-vault/)
- [Static hosting with NOW](https://egghead.io/lessons/tools-deploy-static-assets-with-zeit-s-now)

## Performance

- [Building a Shop with Sub-Second Page Loads](https://medium.baqend.com/building-a-shop-with-sub-second-page-loads-lessons-learned-4bb1be3ed07#.au377wnad)([HN](https://news.ycombinator.com/item?id=12774277))

## Progressive

- [Native apps are doomed](https://medium.com/javascript-scene/native-apps-are-doomed-ac397148a2c0#.inl5qhtin)
- https://dev.opera.com/articles/pwa-resources/

## Management

- [Kaiser](https://medium.com/@pdrummond/introducing-kaiser-204dba2c26ea#.a6j0ig56u) ([My repo](https://github.com/kabootit/kaiser))


## Business

- [SaaS Features](https://www.enterpriseready.io/)
