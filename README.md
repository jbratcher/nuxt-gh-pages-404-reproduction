# Nuxt Github Pages 404 Reproduction

On routes other than the base route, a page refresh results in a 404 error.

I was able to fix the issue by using `generate.fallback` in `nuxt.config.js`

In `nuxt.config.js`:

````javascript
export default {
  generate: {
    fallback: true
  }
}

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
````

For detailed explanation on how things work, check out [Nuxt.js docs](https://nuxtjs.org).
