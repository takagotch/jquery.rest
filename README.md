### jquery.rest
---
https://github.com/jpillora/jquery.rest

```js
var client = new $.RestClient('/rest/api/');
client.add('foo');
client.foo.read();
client.foo.read(42);
clinet.foo.read('forty-two');

var client = new $.RestClient();
client.add();
var request = cliet.foo.read();
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
