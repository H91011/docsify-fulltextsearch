## docsify-fulltextsearch

You can do full text search with this plugin.
Every match list on sidebar and its show which page have matches.

I write this plugin because docsify search plugin is not good and I decide write a good plugin for that.

### Usage:

import plugin and add to docsify: 

```javascirpt

import fullTextSearch from "docsify-fulltextsearch"

```

```javascirpt

window.$docsify = {
  name: '',
  repo: '',
  loadSidebar: true,
  plugins: [
    fullTextSearch
  ]
}

```

For more info please look at o `test` directory.

**If its not work you can directy accsess from "node_modules/docsify-fulltextsearch/index.js"**

### Test

For test :
`npm run test`  

You need to instal docsify-cli before test.

### Config:

You can change match key color and not found text in `index.js`, config object is below:

```javascript

const configs = {
	NO_DATA_TEXT: 'Nothing Found ...',
	RESULT_COLOR: 'yellow',
}

```
