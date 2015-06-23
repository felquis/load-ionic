# Load Ionic

Load diferent versions of Ionic in the browser while debuging
> [Inspiration](http://bocoup.com/weblog/easily-test-jquery-pre-release-versions/)

Instalation
```sh
bower install --save load-ionic
```

Put it in your main HTML exactly where you put your ionic files today
```html
<script src="js/load-ionic.js"></script>
<script>
  // Make sure Ionic was loaded
  if (!window.ionic) {
    document.write('<script src="lib/ionic/js/ionic.bundle.js"><\/script>');
    console.log('Ionic not loaded properly, loading local copy');
  }
</script>
```

It'll load ionic `ionic.bundle.js`

Use param `ionic` in your URL:
> localhost:8100/?ionic=1.0.0

It will load ionic 1.0.0 [from CDN](http://code.ionicframework.com/#)

## .
Please send issues and pull request

## Contribute
Rember to run `npm install` and use `npm run test` to make sure everything is okay.
