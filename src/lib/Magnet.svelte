<script>
  import { getContext } from 'svelte';
  const ctx = getContext('iconCtx') ?? {};
  export let size = ctx.size || '24';
  export let role = ctx.role || 'img';
  export let color = ctx.color || 'currentColor';
  export let ariaLabel = 'magnet';
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
  <path d="M8 2.5H4V5.5H8V2.5Z" fill={color} fill-opacity="0.5" />
  <path d="M20 2.5H16V5.5H20V2.5Z" fill={color} fill-opacity="0.5" />
  <path
    d="M8 7.5H4V13.5C4 17.9183 7.58172 21.5 12 21.5C16.4183 21.5 20 17.9183 20 13.5V7.5H16V13.5C16 15.7091 14.2091 17.5 12 17.5C9.79086 17.5 8 15.7091 8 13.5V7.5Z"
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
@prop export let ariaLabel = 'magnet';
-->
