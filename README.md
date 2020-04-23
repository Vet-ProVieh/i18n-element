# \<i18n-element\>

An Element-Extension to translate it's content. It is written with Vanilla-JS and HTML5-Standards. It recognizes the language of the browser and searching up your translation-keys in a dictonary. You can provide your JSON-Dictonary on your own.

<!-- 
  The next comment block is used by webcomponents.org to enable inline demo.
  Visit https://www.webcomponents.org/publish for more details.
-->
<!--
```
<custom-element-demo>
  <template>
    <script src="../webcomponentsjs/webcomponents-loader.js"></script>
    <link rel="import" href="i18n-element.html">
    <next-code-block></next-code-block>
  </template>
</custom-element-demo>
```
-->
```html
<i18n-element>your.key.to.translate</i18n-element>
```

## 1. Requirements

First of all make sure you have the [Polymer CLI](https://www.npmjs.com/package/polymer-cli) installed. Then run `polymer serve` to serve your element locally.

## 2. Configuration
You had to include your Language-DB as a JSON-File into the HTML-Document. Make sure you have tagged it with `i18n-data`. For example your document looks like this:

```html
<head>
  <link i18n-data rel="import" href="language.html">
</head>
<i18n-element>your.key.to.translate</i18n-element>
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

## Viewing Your Element

```
$ polymer serve --open
```

## Running Tests

```
$ polymer test
```

## Belonging

This web-component belongs to the EFRE research-project Vet:ProVieh from the University of Applied Science Osnabrück.

## License

[MIT](https://opensource.org/licenses/MIT)