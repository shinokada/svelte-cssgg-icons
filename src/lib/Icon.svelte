<script>
  import icons from './icons.js'

  export let name;
  export let width = "24";
  export let height = "24";
  export let strokeWidth = '2';
  export let color = 'currentColor';
  export let role = 'img';
  export let ariaLabel = name;

  $: displayIcon = icons[name]
</script>
<svg
xmlns="http://www.w3.org/2000/svg"
class={$$props.class}
{width}
{height}
fill={color}
{role}
aria-label={ariaLabel}
stroke-linecap="round"
stroke-linejoin="round"
stroke-width={strokeWidth}
{...$$restProps}
on:click
on:keydown
on:keyup
on:focus
on:blur
on:mouseenter
on:mouseleave
on:mouseover
on:mouseout
viewBox="0 0 {displayIcon.box} {displayIcon.box}"
>
  {@html displayIcon.svg}
</svg>

<!--
@component
[Go to Document](https://shinokada.github.io/svelte-evil-icons/)
## Props
@prop name;
@prop width = '50';
@prop height = '50';
@prop strokeWidth = '2';
@prop role = 'img';
@prop color = 'currentColor'
@prop ariaLabel='icon name'
## Event
- on:click
- on:keydown
- on:keyup
- on:focus
- on:blur
- on:mouseenter
- on:mouseleave
- on:mouseover
- on:mouseout
-->