# @crawlo/drivers/ElasticSearch

# ElasticSearch

ElasticSearch is using **elasticsearch** on **npm**

## configure(options, name = 'default')

```js
import ElasticSearch from "@crawlo/drivers/ElasticSearch";

ElasticSearch.configure({
  host: "localhost:9200",
}).then((client) => {
  // client.search({
  //     q: 'keyword'
  // }).then(
  //     body => {
  //     }
  // ).catch(
  //     error => {
  //     }
  // )
});
```

## client

```js
import ElasticSearch from "@crawlo/drivers/ElasticSearch";

ElasticSearch.client
  .search({
    q: "keyword",
  })
  .then((body) => {})
  .catch((error) => {});
```

## getClient(name = 'default')

get a client with name used in configure(options, name)
