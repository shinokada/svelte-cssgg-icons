# Svelte Cssgg Icons

<div class="flex gap-2 my-8">
<a href="https://github.com/sponsors/shinokada" target="_blank"><img src="https://img.shields.io/static/v1?label=Sponsor&message=%E2%9D%A4&logo=GitHub&color=%23fe8e86" alt="sponsor" height="25" style="height: 25px !important;"></a>
<a href="https://www.npmjs.com/package/svelte-cssgg-icons" rel="nofollow" target="_blank"><img src="https://img.shields.io/npm/v/svelte-cssgg-icons" alt="npm" height="25" style="height: 25px !important;"></a>
<a href="https://twitter.com/shinokada" rel="nofollow" target="_blank"><img src="https://img.shields.io/badge/created%20by-@shinokada-4BBAAB.svg" alt="Created by Shin Okada" height="25" style="height: 25px !important;"></a>
<a href="https://opensource.org/licenses/MIT" rel="nofollow" target="_blank"><img src="https://img.shields.io/github/license/shinokada/svelte-cssgg-icons" alt="License" height="25" style="height: 25px !important;"></a>
<a href="https://www.npmjs.com/package/svelte-cssgg-icons" rel="nofollow" target="_blank"><img src="https://img.shields.io/npm/dw/svelte-cssgg-icons.svg" alt="npm" height="25" style="height: 25px !important;"></a>
</div>

700+ SVG icons from <a href="https://github.com/astrit/css.gg">css.gg</a> for Svelte.

Thank you for considering my open-source package. If you use it in a commercial project, please support me by sponsoring me on GitHub: https://github.com/sponsors/shinokada. Your support helps me maintain and improve this package for the benefit of the community.

## Repo

[GitHub repo](https://github.com/shinokada/svelte-cssgg-icons)

## Original source

[astrit/css.gg](https://github.com/astrit/css.gg)

## License

[Svelte-Cssgg-Icons License](https://github.com/shinokada/svelte-cssgg-icons/LICENSE)

[Css.gg License](https://github.com/astrit/css.gg/blob/master/LICENSE)

## Installation

```sh
pnpm i -D svelte-cssgg-icons
```

## Usage

In a svelte file:

```html
<script>
  import { Icon } from 'svelte-cssgg-icons';
</script>

<Icon name="add" />
```

## Props

- @prop name;
- @prop width = '50';
- @prop height = '50';
- @prop strokeWidth = '2';
- @prop role = 'img';
- @prop color = 'currentColor'
- @prop ariaLabel='icon name'

## IDE support

If you are using an LSP-compatible editor, such as VSCode, Atom, Sublime Text, or Neovim, hovering over a component name will display a documentation link, features, props, events, and an example.


## Size

Use the `width` and `height` props to change the size of icons.

```html
<Icon name="add" width="100" height="100" />
```

If you are using Tailwind CSS, you can add a custom size using Tailwind CSS by including the desired classes in the `class` prop. For example:

```html
<Icon name="add" class="shrink-0 h-20 w-20" />
```

## CSS HEX Colors

Use the `color` prop to change colors with HEX color code.

```html
<Icon name="add" color="#c61515" />
```

## CSS framworks suport

You can apply CSS framework color and other attributes directly to the icon component or its parent tag using the `class` prop.

Tailwind CSS example:

```html
<Icon name="add" class="text-red-700 inline m-1" />
```

Bootstrap examples:

```html
<Icon name="add" class="position-absolute top-0 px-1" />
```

## Dark mode

If you are using the dark mode on your website with Tailwind CSS, add your dark mode class to the `class` prop.

Let's use `dark` for the dark mode class as an example.

```html
<Icon name="add" class="text-red-700 dark:text-green-500" />
```

## aria-label

All icons have aria-label. For example `bell` has `aria-label="bell"`.
Use `ariaLabel` prop to modify the `aria-label` value.

```html
<Icon name="add" ariaLabel="red bell" color="#c61515"/>
```

## Unfocusable icon

If you want to make an icon unfocusable, add `tabindex="-1"`.

```html
<Icon name="add" tabindex="-1" />
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
<Icon name="add" tabindex="0" />
```

## Using svelte:component

```html
<svelte:component this="{Icon}" name="add"/>
```

## Using onMount

```html
<script>
  import {Icon} from 'svelte-cssgg-icons';
  import { onMount } from 'svelte';
  const props = {
    name: 'arrow-down',
    size: '50',
    color: '#ff0000'
  };
  onMount(() => {
    const icon = new Icon({ target: document.body, props });
  });
</script>
```

## Import all

Use `import {Icon, icons} from 'svelte-cssgg-icons';`.

```html
<script>
  import {Icon, icons} from 'svelte-cssgg-icons';
</script>

{#each Object.keys(icons) as name}
<div class="flex gap-4 items-center text-lg">
  <Icon name={name} bind:width={size} bind:height={size} class="shrink-0"/>
  {name}
</div>
{/each}
```

## Other icons

- [Svelte-Icon-Sets](https://svelte-svg-icons.vercel.app/)

