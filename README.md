# pouchdb-adapter-dynamodb
PouchDB adapter for DynamoDB
=====

PouchDB adapter using [dynamodbdown](https://github.com/KlausTrainer/dynamodbdown) the dynamodb plugin for levelup. Designed for running a quick persistent PouchDB adapter in Node.js.

**Warning: not designed for production use.** 

Usage
----

Install:

    npm install pouchdb-adapter-dynamodb

Then

```js
var PouchDB = require('pouchdb-core')
  .plugin(require('pouchdb-adapter-dynamodb'));

var db = new PouchDB('mydb', {adapter: 'dynamodb'});
```

Testing
--------

```
COUCH_HOST=http://admin:secret@localhost:5984 npm test
```
