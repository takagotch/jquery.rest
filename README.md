### jquery.rest
---
https://github.com/jpillora/jquery.rest

```js
var client = new $.RestClient('/rest/api/');
client.add('foo');
client.foo.read();
client.foo.read(42);
clinet.foo.read('forty-two');



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
```

```
{
  'create': 'POST',
  'read': 'GET',
  'update': 'PUT',
  'delete': 'DELETE ',
}
```

```
<script src="ajax.googleapis.com/ajax/libs/jquery/1/jquery.min.js"></script>
<script src="http://jpillora.com/jquery.rest/dist/1/jquery.rest.min.js"></script>
```
