# Tame Your Theme

[![https://github.com/wellgrisa/tame-your-theme/workflows/.github/workflows/main.yml/badge.svg](https://github.com/wellgrisa/tame-your-theme/workflows/.github/workflows/main.yml/badge.svg)](https://github.com/wellgrisa/tame-your-theme/actions/workflows/main.yml)

## Overview

For the [full and interactive documentation go here](https://wellgrisa.github.io/tame-your-theme/).

The main idea of this lib is to help creating themes by using [CSS custom variables](https://developer.mozilla.org/en-US/docs/Web/CSS/Using_CSS_custom_properties#Inheritance_of_CSS_Variables) alongside with [HSL](https://vanseodesign.com/web-design/hue-saturation-and-lightness/) colors and the [CSS Object Model](https://developer.mozilla.org/en-US/docs/Web/API/CSS_Object_Model) to change the css variables in runtime.

To achieve that, this lib is split in two packages:

- `@tame-your-theme/scss` - scss helper functions to create themed css variable colors, themed color harmonies
- `@tame-your-theme/css-style-declaration` - native css style declarations api helper to change theme in run time

Each package can be used independently.

If you don't need to change in run time, you can just use the [`@tame-your-theme/scss`](https://www.npmjs.com/package/@tame-your-theme/scss) to create your variables and play with its colors easily.

## Installation

Using npm:

```
npm install @tame-your-theme/css-style-declaration
npm install @tame-your-theme/scss
```

Using yarn:

```
yarn add @tame-your-theme/css-style-declaration
yarn add @tame-your-theme/scss
```

## TL;DR

How to use in just a few steps:

- create the themed colors by using the mixin `create-theme-color` from the `@tame-your-theme/scss`
- create the themes using a list of names and values in your javascript preferred language (typescript, vanilla, react, angular...)
- call the `setTheme` from the `@tame-your-theme/css-style-declaration` with the desired theme

Each package might be used independently, though they are thought of being used together.

For more details check each package's Readme, but mostly the [full and interactive documentation go here](https://wellgrisa.github.io/tame-your-theme/).
