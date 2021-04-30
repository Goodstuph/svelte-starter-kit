
# svelte starter kit

This is a project template for [Svelte](https://svelte.dev) apps. It lives at https://github.com/Goodstuph/svelte-starter-kit.

To create a new project based on this template using [degit](https://github.com/Rich-Harris/degit):

```bash
npx degit Goodstuph/svelte-starter-kit svelte-app
cd svelte-app
```

*Note that you will need to have [Node.js](https://nodejs.org) installed.*


## Get started

Install the dependencies...

```bash
cd svelte-app
npm install
```

...then start [Rollup](https://rollupjs.org):

```bash
npm run dev
```

Navigate to [localhost:5000](http://localhost:5000). You should see your app running. Edit a component file in `src`, save it, and reload the page to see your changes.

## Defaults 

There are some differences from the official [svelte template](https://github.com/sveltejs/template). For instance, we have added functionality _akin to env variables_ in the `rollup.config.js` file. It basically offers replacements. 

Additionally, we've set this up to use `svelte-preprocess` to use *scss*. There is a global scss file in the `styles` folder. Everything in that file will be pre-pended to the code. You can also add multiple more files and just import it into the global file. 

**Routing** has been added through [svelte-routing](https://github.com/EmilTholin/svelte-routing).

By default, the server will only respond to requests from localhost. To allow connections from other computers, edit the `sirv` commands in package.json to include the option `--host 0.0.0.0`.

## Building and running in production mode

To create an optimised version of the app:

```bash
npm run build
```

You can run the newly built app with `npm run start`. This uses [sirv](https://github.com/lukeed/sirv), which is included in your package.json's `dependencies`.


## Things to add maybe 
[] separate branch for layout component
[] separate branch to show usage with Stores

## Deploying to the web

### With [Vercel](https://vercel.com)

Install `vercel` if you haven't already:

```bash
npm install -g vercel
```

Then, from within your project folder:

```bash
cd public
vercel deploy --name my-project
```

### With [surge](https://surge.sh/)

Install `surge` if you haven't already:

```bash
npm install -g surge
```

Then, from within your project folder:

```bash
npm run build
surge public my-project.surge.sh
```
