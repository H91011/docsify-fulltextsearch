## docsify-fulltextsearch

You can do full text search with this plugin.
Every match list on sidebar and its show which page have matches.

I write this plugin because docsify search plugin is not good and I decide write a good plugin for that.

### Usage:
Copy `index.js` to `index.html` directory an add like below: 

In `./test/index.html`:
```javascirpt

  <script src="index.js"></script>
  <script>

    setFullTextSearchConfig({
      NO_DATA_TEXT: 'sorry I cant found anything...',
      RESULT_COLOR: 'violet',
      INSENSITIVE: true
    })
    
    window.$docsify = {
      name: '',
      repo: '',
      loadSidebar: true,
      plugins: [
        fullTextSearch
      ]
    }
  </script>

```

For more info please look at o `test` directory.

**If its not work you can directy accsess from "node_modules/docsify-fulltextsearch/index.js"**

### Test

You need to instal docsify-cli before test.

For test :
`npm install -g docsify-cli`
`npm run test`  

### Config:

Default config values:

```javascript

const configs = {
  NO_DATA_TEXT: 'Nothing Found ...',
  RESULT_COLOR: 'yellow',
  INSENSITIVE: false
}

```

You can change with `setFullTextSearchConfig`

```javascript

// change multiple
setFullTextSearchConfig({
  NO_DATA_TEXT: 'sorry I cant found anything...',
  RESULT_COLOR: 'violet',
  INSENSITIVE: true
})

//or single: 
setFullTextSearchConfig({
  RESULT_COLOR: 'violet',
})

```


