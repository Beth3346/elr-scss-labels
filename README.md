# elr-scss-labels

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![npm](https://img.shields.io/npm/dm/elr-scss-labels.svg?style=flat)](https://npmjs.com/package/elr-scss-labels)

a library of sass mixins

## Installation

Download node at [nodejs.org](http://nodejs.org) and install it, if you haven't already.

```sh
npm install elr-scss-labels --save
yarn add elr-scss-labels
```

## Documentation

```scss
@import "elr-scss-labels/src/main";
```

### Basic Label

```scss
.elr-label {
  @include elr-label;
  margin: 10px 5px;
}
```

```html
<div class="elr-label">
  <span class="elr-label-icon"><i class="fa fa-heart"></i></span>
  <span class="elr-label-title">Label</span>
  <span class="elr-label-value">10</span>
</div>
```

### Pill Label

```scss
.elr-pill-label {
  @include elr-label(
    $config: (
      border-radius: 30px,
    )
  );
}
```

```html
<div class="elr-pill-label">
  <span class="elr-label-title">Pill Label</span>
</div>
```

```scss
.elr-label-info {
  @include elr-label-context(
    $config: (
      type: "info",
    )
  );
}
```

```html
<div class="elr-label elr-label-info"><span>Information</span></div>
```

```scss
.elr-label-danger {
  @include elr-label-context(
    $config: (
      type: "danger",
    )
  );
}
```

```html
<div class="elr-label elr-label-danger"><span>Danger</span></div>
```

```scss
.elr-label-warning {
  @include elr-label-context(
    $config: (
      type: "warning",
    )
  );
}
```

```html
<div class="elr-label elr-label-warning"><span>Warning</span></div>
```

```scss
.elr-label-success {
  @include elr-label-context(
    $config: (
      type: "success",
    )
  );
}
```

```html
<div class="elr-label elr-label-success"><span>Success</span></div>
```

```scss
.elr-label-muted {
  @include elr-label-context(
    $config: (
      type: "muted",
    )
  );
}
```

```html
<div class="elr-label elr-label-muted"><span>Muted</span></div>
```

### Dismissible Labels

```html
<div class="elr-label">
  <span class="elr-label-title">Click Here</span>
  <button>
    <span class="fa fa-times elr-label-close" />
  </button>
</div>
```

## License SEE LICENSE IN LICENSE.md
