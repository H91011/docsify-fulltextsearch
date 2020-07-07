## docsify-fulltextsearch

You can do full text search with this plugin.
Every match list on sidebar and its show which page have matches.

I write this plugin because docsify search plugin is not good and I decide write a good plugin for that.

### Usage:

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

### Test

For test :
`npm run test`  

You need to instal docsify-cli before test.

### Config:

You can change match key color and not found text in `search.js`, config object is below:

```javascript

const configs = {
	NO_DATA_TEXT: 'Nothing Found ...',
	RESULT_COLOR: 'yellow',
}

```
