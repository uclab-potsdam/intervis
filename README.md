# Intervis

## Build Setup

```bash
# install dependencies
$ npm install

# serve with hot reload at localhost:3000
$ npm run dev

# build for production and launch server
$ npm run build
$ npm run start

# generate static project
$ npm run generate
```

For detailed explanation on how things work, check out [Nuxt.js docs](https://nuxtjs.org).


## Update content and deploy new version to UCLAB server

Update content:
- Start dev environment if you want to use auto-fixing eslint issues ($ npm run dev, see Build Setup above)
- Run juypter notebook _data-processing.ipynb in ./data directory to download current content version and create the language files

Deploy current version to UCLAB server:
- Run $ npm run generate:uclab
- Upload content of ./dist directory to /public/intervis. Make sure, you do not replace the instrumentation dir holding the log files
