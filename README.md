<h1 align="center">Svelte Cssgg Icons</h1>

<p align="center">
<a href="https://github.com/shinokada/cssgg-icons">Svelte-Cssgg-Icons</a>
</p>

<p align="center">
<a href="https://github.com/sponsors/shinokada" target="_blank"><img src="https://img.shields.io/static/v1?label=Sponsor&message=%E2%9D%A4&logo=GitHub&color=%23fe8e86" height="25"></a>
<a href="https://www.npmjs.com/package/svelte-cssgg-icons" rel="nofollow" target="_blank"><img src="https://img.shields.io/npm/v/svelte-cssgg-icons" alt="npm" height="25"></a>
<a href="https://twitter.com/shinokada" rel="nofollow" target="_blank"><img src="https://img.shields.io/badge/created%20by-@shinokada-4BBAAB.svg" alt="Created by Shin Okada" height="25"></a>
<a href="https://opensource.org/licenses/MIT" rel="nofollow" target="_blank"><img src="https://img.shields.io/github/license/shinokada/svelte-cssgg-icons" alt="License" height="25"></a>
<a href="https://www.npmjs.com/package/svelte-cssgg-icons" rel="nofollow" target="_blank"><img src="https://img.shields.io/npm/dw/svelte-cssgg-icons.svg" alt="npm" height="25"></a>
</p>

700+ SVG icons from <a href="https://github.com/astrit/css.gg">css.gg</a> for Svelte.

Thank you for considering my open-source package. If you use it in a commercial project, please support me by sponsoring me on GitHub: https://github.com/sponsors/shinokada. Your support helps me maintain and improve this package for the benefit of the community.

<p align="center">
<img src="https://raw.githubusercontent.com/shinokada/cssgg-icons/main/static/images/svelte-cssgg-icons-color-450.webp" width="450" />
</p>

## Installation

```sh
npm i -D svelte-cssgg-icons
```

## Icon list

[Icon list](/icon-list.md)

## Icon images

[Icon images](/icon-images.md)

## Usage

In a svelte file:

```html
<script>
  import { Add } from 'svelte-cssgg-icons';
</script>

<Add />
```

## Faster compiling

If you need only a few icons from this library in your Svelte app, import them directly. This can optimize compilation speed and improve performance by reducing the amount of code processed during compilation.

```html
<script>
  import Add from 'svelte-cssgg-icons/Add.svelte';
</script>

<Add />
```

If you are a TypeScript user, install **typescript version 5.0.0 or above**.

```sh
pnpm i -D typescript@latest
```

To avoid any complaints from the editor, add `node16` or `nodenext` to `moduleResolution` in your tsconfig.json file.

```json
{
  //...
  "compilerOptions": {
    // ...
    "moduleResolution": "nodenext"
  }
}
```

## REPL

- [Demo color](https://svelte.dev/repl/36584bc35f364444893640b660723f80?version=4.0.1)
- [Demo mono](https://svelte.dev/repl/77dd916fe61a42f2a01b84d9e89033a4?version=4.0.1)

## Props

- color = 'currentColor';
- size = '24';
- role = 'img';
- ariaLabel = 'file name';

## IDE support

If you are using an LSP-compatible editor, such as VSCode, Atom, Sublime Text, or Neovim, hovering over a component name will display a documentation link, features, props, events, and an example.

## Size

Use the `size` prop to change the size of icons.

```html
<script>
  import { Add } from 'svelte-cssgg-icons';
</script>

<Add size="30" />
```

## CSS HEX Colors

Use the `color` prop to change colors with HEX color code.

```html
<BxAbacus color="#c61515" />
```

## CSS frameworks suport

Use the `class` prop to change colors and add additional css.

Tailwind example:

```html
<script>
  import { Add } from 'svelte-cssgg-icons';
</script>

<Add class="m-8" />
```

Bootstrap example:

```html
<Add class="px-4" />
```

## Unfocusable icon

If you want to make an icon unfocusable, add `tabindex="-1"`.

```html
<Add tabindex="-1" />
```

## Events

All icons have the following events:

- on:click
- on:keydown
- on:keyup
- on:focus
- on:blur
- on:mouseenter
- on:mouseleave
- on:mouseover
- on:mouseout

## Passing down other attributes

You can pass other attibutes as well.

```html
<Add tabindex="0" />
```

## Using svelte:component

```html
<script>
  import { Add } from 'svelte-cssgg-icons';
</script>

<svelte:component this="{Add}" />
```

## Import all

[REPL](https://svelte.dev/repl/6b2057d58c3841fc9f37b67960f02e27)

Use `import * as Icon from 'svelte-cssgg-icons`.

```html
<script>
  import * as Icon from 'svelte-cssgg-icons';
</script>

<h1>Size</h1>
<Icon.Add size="30" />
<Icon.Add size="40" />
<Icon.Add size="50" />

<h1>Tailwind CSS</h1>
<Icon.Add class="m-4" />
<Icon.Add class="m-8" />
```

## Other icons

- [Svelte-Icon-Sets](https://svelte-svg-icons.vercel.app/)
