# [vue-wordpress-pwa](https://www.fullstackweekly.com/category/blog)

> An offline-first SPA using Vue.js, the WordPress REST API and Progressive Web Apps

## Getting Started

### Prerequisites

Make sure that [Node v11](https://nodejs.org/en/download/releases/) is installed.

## Features

- Modern JavaScript syntax with [ES6](https://github.com/lukehoban/es6features) via [babel](https://babeljs.io/).
- Module bundler via [webpack](https://webpack.github.io/).
- Components-based architecture via [Vue.js](https://vuejs.org/).
- State management via [Vuex](https://vuex.vuejs.org/en/).
- Cache busting via [file-loader](https://webpack.github.io/)
- Progressive Web App enabled with [service workers](https://developers.google.com/web/fundamentals/getting-started/primers/service-workers)
- Offline capable with [service workers, app cache](https://developers.google.com/web/fundamentals/getting-started/primers/service-workers)
- CSS with [Sass](http://sass-lang.com/)

### Instructions

First, install the WordPress plugins to enhance its REST API

- Better REST API Featured Images
- REST API Enabler
- WP REST API - filter fields
- WP REST API - Pure Taxonomies

Then, clone the repo or create a fork

```bash
$ git clone https://github.com/bstavroulakis/vue-wordpress-pwa.git
```

Then, edit the config:

```bash
src/app.config.js
```

Then, edit the theme, routes and assets:

```bash
src/theme/
src/components/routerTypes.js
src/components/router.js
src/assets
```

Finally, to run the project for development with hot reload:

```bash
$ npm install
$ npm run dev
```

Or, build the project for production:

```bash
$ npm run build
```

### Deployment

Setup a new site on Azure App Services https://[fullstackweekly].azurewebsites.net
and as the path select your forked Github project.

Your site should be running on the path you created (https://[fullstackweekly].azurewebsites.net)!

It should work offline as well and with every commit it will deploy the changes to Azure.
Once the user refreshes the site he will receive the new cached version `immediately`.

License

MIT
