## WEB API 使う
* アクセストークン付きで REST API を呼び出すだけ!

```javascript
$.ajax({
  url: 'https://public-api.wordpress.com/rest/v1/sites/masakura.wordpress.com/posts/',
  type: 'GET',
  beforeSend: function (xhr) {
    xhr.setRequestHeader('Authorization', 'BEARER ' + access_token);
  }
})
.done(function (result) {
  // ここになんか書く...
});
```
