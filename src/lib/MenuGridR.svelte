<script>
  import { getContext } from 'svelte';
  const ctx = getContext('iconCtx') ?? {};
  export let size = ctx.size || '24';
  export let role = ctx.role || 'img';
  export let color = ctx.color || 'currentColor';
  export let ariaLabel = 'menu grid r';
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
  <path d="M4 4H8V8H4V4Z" fill={color} />
  <path d="M4 10H8V14H4V10Z" fill={color} />
  <path d="M8 16H4V20H8V16Z" fill={color} />
  <path d="M10 4H14V8H10V4Z" fill={color} />
  <path d="M14 10H10V14H14V10Z" fill={color} />
  <path d="M10 16H14V20H10V16Z" fill={color} />
  <path d="M20 4H16V8H20V4Z" fill={color} />
  <path d="M16 10H20V14H16V10Z" fill={color} />
  <path d="M20 16H16V20H20V16Z" fill={color} />
</svg>

<!--
@component
[Go to docs](https://svelte-cssgg-icons.vercel.app)
## Props
@prop export let size = ctx.size || '24';
@prop export let role = ctx.role || 'img';
@prop export let color = ctx.color || 'currentColor';
@prop export let ariaLabel = 'menu grid r';
-->
