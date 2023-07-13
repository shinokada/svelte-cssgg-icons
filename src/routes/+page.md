# Svelte Cssgg Icons

<div class="flex justify-center gap-2 my-8">
<a href="https://github.com/sponsors/shinokada" target="_blank"><img src="https://img.shields.io/static/v1?label=Sponsor&message=%E2%9D%A4&logo=GitHub&color=%23fe8e86" height="25" style="height: 25px !important;"></a>
<a href="https://www.npmjs.com/package/svelte-cssgg-icons" rel="nofollow" target="_blank"><img src="https://img.shields.io/npm/v/svelte-cssgg-icons" alt="npm" height="25" style="height: 25px !important;"></a>
<a href="https://twitter.com/shinokada" rel="nofollow" target="_blank"><img src="https://img.shields.io/badge/created%20by-@shinokada-4BBAAB.svg" alt="Created by Shin Okada" height="25" style="height: 25px !important;"></a>
<a href="https://opensource.org/licenses/MIT" rel="nofollow" target="_blank"><img src="https://img.shields.io/github/license/shinokada/svelte-cssgg-icons" alt="License" height="25" style="height: 25px !important;"></a>
<a href="https://www.npmjs.com/package/svelte-cssgg-icons" rel="nofollow" target="_blank"><img src="https://img.shields.io/npm/dw/svelte-cssgg-icons.svg" alt="npm" height="25" style="height: 25px !important;"></a>
</div>

700+ SVG icons from <a href="https://github.com/astrit/css.gg">css.gg</a> for Svelte.

Thank you for considering my open-source package. If you use it in a commercial project, please support me by sponsoring me on GitHub: https://github.com/sponsors/shinokada. Your support helps me maintain and improve this package for the benefit of the community.

## Repo

[GitHub repo](https://github.com/shinokada/svelte-cssgg-icons)

## Installation

```sh
pnpm i -D svelte-cssgg-icons
```

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

If you are using Tailwind CSS, you can add a custom size using Tailwind CSS by including the desired classes in the `class` prop. For example:

```html
<Add class="shrink-0 h-20 w-20" />
```

## CSS HEX Colors

Use the `color` prop to change colors with HEX color code.

```html
<BxAbacus color="#c61515" />
```

## CSS frameworks suport

You can apply CSS framework color and other attributes directly to the icon component or its parent tag using the `class` prop.

Tailwind example:

```html
<script>
  import { Add } from 'svelte-cssgg-icons';
</script>

<Add class="text-red-700 dark:text-green-300 inline m-1" />
```

Bootstrap example:

```html
<Add class="px-4" />
```

## Dark mode

If you are using the dark mode on your website with Tailwind CSS, add your dark mode class to the `class` prop.

Let's use `dark` for the dark mode class as an example.

```html
<Add class="text-blue-700 dark:text-red-500" />
```

## aria-label

All icons have aria-label. For example `EiBell` has `aria-label="ei bell"`.
Use `ariaLabel` prop to modify the `aria-label` value.

```html
<Add ariaLabel="ei bell" />
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

## Using onMount

```html
<script>
  import { EiBell } from 'svelte-evil-icons';
  import { onMount } from 'svelte';
  const props = {
    size: '50',
    color: '#ff0000'
  };
  onMount(() => {
    const icon = new EiBell({ target: document.body, props });
  });
</script>
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
