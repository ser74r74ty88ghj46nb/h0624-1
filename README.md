[![Deploy](https://www.herokucdn.com/deploy/button.png)](https://dashboard.heroku.com/new?template=https://github.com/ser74r74ty88ghj46nb/h0624-1.git)

```
addEventListener(
  "fetch", event => {
    let url = new URL(event.request.url);
    url.host = "appname.herokuapp.com";
    let request = new Request(url, event.request);
    event.respondWith(
      fetch(request)
    )
  }
)
```
