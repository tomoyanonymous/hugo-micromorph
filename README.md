# hugo-micromorph

Dead simple module to use [micromorph] in hugo to pre-fetch pages.

https://github.com/natemoo-re/micromorph

## Usage

### Install

On your site config(`hugo.toml` for instance), add the module import line.

```toml
[[module.imports]]
path = 'github.com/tomoyanonymous/hugo-micromorph
```

and download it.

```sh
hugo mod get -u
```

Before start building site, you need to install npm modules.

```sh
hugo mod npm pack
npm install
```

### Template

In your template, insert the partial before the end of `<body>` tag.

```
{{ partialCached "micromorph.html" . }}
```


## Author

Tomoya Matsuura

## [License](./LICENSE)