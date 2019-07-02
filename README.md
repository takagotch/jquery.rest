### jquery.rest
---
https://github.com/jpillora/jquery.rest

```js
var client = new $.RestClient('/rest/api/');
client.add('foo');
client.foo.read();
client.foo.read(42);
clinet.foo.read('forty-two');

var client = new $.RestClient('/rest/api');

client.add('foo');

var request = client.foo.read();
request.done(function (data, textStatus, xhrObject) {
  alert('I have data: ' + data);
});

client.foo.read().done(function (data) {
  alert('I have data: ' + data);
});

var client = new $.RestClient('/rest/api/');

client.add('foo');
client.foo.add('baz');
client.foo.read();
client.foo.read(42);
client.foo.baz.read();
client.foo.baz.read(42);
client.foo.baz.('forty-two', 21);

var client = new $.RestClient('/rest/api/');
client.add('forum');
client.forum.add('post');
client.forum.post.add('comment');

var comment = client.forum.post.comment;
comment.read(42,21,7);
comment.update(42,21,7, {...});

$.client = new $.RestClient('/rest/api/');
$.client.add('foo');

var client = new $.RestClient('/rest/api/');
client.add('foo');
var request = cliet.foo.read(42);
request.done(funciton (data, textStatus, xhrObject){
  alert('I have data: ' + data);
});

request: function(resource, options) {
  return $.ajax(options);
}

var client = new $.RestClient('/rest/api/');

client.add('add');
client.foo.add('bar', { isSingle: true });
client.foo.bar.add('baz');

client.foo.bar.bazz.read(42, 21);

var clinet = new $.RestClient('/rest/api/');
client.add('foo');

clinet.foo.read();
client.foo.read(42);

client.foo.update(42, {my: "updates"});
client.foo.destroy(42);
client.foo.del(42);

```

```json
{
  'create': 'POST',
  'read': 'GET',
  'update': 'PUT',
  'delete': 'DELETE ',
}
```

```html
<script src="ajax.googleapis.com/ajax/libs/jquery/1/jquery.min.js"></script>
<script src="http://jpillora.com/jquery.rest/dist/1/jquery.rest.min.js"></script>
```
