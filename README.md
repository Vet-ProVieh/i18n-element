
# i18n-translate: Web-Component for Translation

An Element-Extension to translate it's content. It is written with Vanilla-JS and HTML5-Standards. It recognizes the language of the browser and searching up your translation-keys in a dictonary. You can provide your JSON-Dictonary on your own.

It's not as complex as other i18n-components, but it is simple and extendable. This project is at an early stage and needs further development.

<!-- 
  The next comment block is used by webcomponents.org to enable inline demo.
  Visit https://www.webcomponents.org/publish for more details.
-->
<!--
```
<custom-element-demo>
  <template>
    <script src="../webcomponentsjs/webcomponents-loader.js"></script>
    <link i18n-data rel="import" href="demo/language.html">
    <link rel="import" href="i18n-translate.html">
  </template>
</custom-element-demo>
```
-->
```html
    <p>Firstname: <i18n-translate>person.firstname</i18n-translate></p>
    <p>Lastname: <i18n-translate>person.lastname</i18n-translate></p>
    <p>Not-Known: <i18n-translate>unkown</i18n-translate></p>
```

## 1. Requirements

First of all make sure you have the [Polymer CLI](https://www.npmjs.com/package/polymer-cli) installed. Then run `polymer serve` to serve your element locally.

## 2. Configuration
You had to include your Language-DB as a JSON-File into the HTML-Document. Make sure you have tagged it with `i18n-data`. For example your document looks like this:

```html
<head>
  <link i18n-data rel="import" href="language.html">
</head>
<i18n-translate>your.key.to.translate</i18n-translate>
```

So your `language.html` should contain the following:

```json
{
  "en": {
    "your": {
      "key": {
        "to": {
          "translate
        }
      }
    }
  }
}
```

## 3. Installation

```npm i @tomuench/i18n-translate```

# Development
In the following section it is described how to extend this web-component.

## Viewing Your Element

```
$ polymer serve --open
```

## Running Tests

```
$ polymer test
```

## Contributing
1. Fork it!
2. Create your feature branch: git checkout -b my-new-feature
3. Commit your changes: git commit -am 'Add some feature'
4. Push to the branch: git push origin my-new-feature
5. Submit a pull request :D

## Credits

This web-component belongs to the EFRE research-project Vet:ProVieh from the University of Applied Science Osnabrück.

Thanks to Adam Bien for his inspriation in the blog-entry http://www.adam-bien.com/roller/abien/entry/simplest_possible_internationalization_with_vanilla. 

## License

[MIT](https://opensource.org/licenses/MIT)