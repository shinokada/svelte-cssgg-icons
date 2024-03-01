<script>
  import { getContext } from 'svelte';
  const ctx = getContext('iconCtx') ?? {};
  export let size = ctx.size || '24';
  export let role = ctx.role || 'img';
  export let color = ctx.color || 'currentColor';
  export let ariaLabel = 'menu oreos';
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
  <path d="M7 3C5.34315 3 4 4.34315 4 6H20C20 4.34315 18.6569 3 17 3H7Z" fill={color} />
  <path d="M7 11C5.34315 11 4 9.65685 4 8H20C20 9.65685 18.6569 11 17 11H7Z" fill={color} />
  <path d="M7 13C5.34315 13 4 14.3431 4 16H20C20 14.3431 18.6569 13 17 13H7Z" fill={color} />
  <path d="M7 21C5.34315 21 4 19.6569 4 18H20C20 19.6569 18.6569 21 17 21H7Z" fill={color} />
</svg>

<!--
@component
[Go to docs](https://svelte-cssgg-icons.codewithshin.com)
## Props
@prop export let size = ctx.size || '24';
@prop export let role = ctx.role || 'img';
@prop export let color = ctx.color || 'currentColor';
@prop export let ariaLabel = 'menu oreos';
-->
