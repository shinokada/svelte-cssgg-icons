<script>
  import { getContext } from 'svelte';
  const ctx = getContext('iconCtx') ?? {};
  export let size = ctx.size || '24';
  export let role = ctx.role || 'img';
  export let color = ctx.color || 'currentColor';
  export let ariaLabel = 'drop invert';
</script>

<svg
  width={size}
  height={size}
  {role}
  {...$$restProps}
  aria-label={ariaLabel}
  on:click
  on:keydown
  on:keyup
  on:focus
  on:blur
  on:mouseenter
  on:mouseleave
  on:mouseover
  on:mouseout
  viewBox="0 0 24 24"
  fill="none"
  xmlns="http://www.w3.org/2000/svg"
>
  <path
    fill-rule="evenodd"
    clip-rule="evenodd"
    d="M12.0001 1.13611L5.63604 7.50002C2.12132 11.0147 2.12132 16.7132 5.63604 20.2279C7.39343 21.9853 9.69679 22.864 12.0001 22.864C12.288 22.864 12.5759 22.8502 12.8627 22.8228C14.8706 22.6306 16.8264 21.7657 18.3641 20.2279C21.8788 16.7132 21.8788 11.0147 18.3641 7.50002L12.0001 1.13611ZM7.05025 8.91423L12 3.96448L12.0001 20.864C10.2086 20.864 8.41711 20.1806 7.05025 18.8137C4.31658 16.0801 4.31658 11.6479 7.05025 8.91423Z"
    fill={color}
  />
</svg>

<!--
@component
[Go to docs](https://svelte-cssgg-icons.codewithshin.com)
## Props
@prop export let size = ctx.size || '24';
@prop export let role = ctx.role || 'img';
@prop export let color = ctx.color || 'currentColor';
@prop export let ariaLabel = 'drop invert';
-->
