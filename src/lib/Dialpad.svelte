<script>
  import { getContext } from 'svelte';
  const ctx = getContext('iconCtx') ?? {};
  export let size = ctx.size || '24';
  export let role = ctx.role || 'img';
  export let color = ctx.color || 'currentColor';
  export let ariaLabel = 'dialpad';
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
  <path d="M5.5 3H8.5V6H5.5V3Z" fill={color} />
  <path d="M5.5 8H8.5V11H5.5V8Z" fill={color} />
  <path d="M5.5 13V16H8.5V13H5.5Z" fill={color} />
  <path d="M10.5 3H13.5V6H10.5V3Z" fill={color} />
  <path d="M10.5 8V11H13.5V8H10.5Z" fill={color} />
  <path d="M10.5 13H13.5V16H10.5V13Z" fill={color} />
  <path d="M10.5 18V21H13.5V18H10.5Z" fill={color} />
  <path d="M15.5 3H18.5V6H15.5V3Z" fill={color} />
  <path d="M15.5 8V11H18.5V8H15.5Z" fill={color} />
  <path d="M15.5 13H18.5V16H15.5V13Z" fill={color} />
</svg>

<!--
@component
[Go to docs](https://svelte-cssgg-icons.codewithshin.com)
## Props
@prop export let size = ctx.size || '24';
@prop export let role = ctx.role || 'img';
@prop export let color = ctx.color || 'currentColor';
@prop export let ariaLabel = 'dialpad';
-->
