<script>
  import { getContext } from 'svelte';
  const ctx = getContext('iconCtx') ?? {};
  export let size = ctx.size || '24';
  export let role = ctx.role || 'img';
  export let color = ctx.color || 'currentColor';
  export let ariaLabel = 'volume';
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
    d="M24 12C24 16.4183 20.4183 20 16 20V18C19.3137 18 22 15.3137 22 12C22 8.68629 19.3137 6 16 6V4C20.4183 4 24 7.58172 24 12Z"
    fill={color}
  />
  <path
    d="M20 12C20 14.2091 18.2091 16 16 16V14C17.1046 14 18 13.1046 18 12C18 10.8954 17.1046 10 16 10V8C18.2091 8 20 9.79086 20 12Z"
    fill={color}
  />
  <path
    fill-rule="evenodd"
    clip-rule="evenodd"
    d="M9 16L15 20V4L9 8H5C2.79086 8 1 9.79086 1 12C1 14.2091 2.79086 16 5 16H9ZM5 10H9L13 7.5V16.5L9 14H5C3.89543 14 3 13.1046 3 12C3 10.8954 3.89543 10 5 10Z"
    fill={color}
  />
</svg>

<!--
@component
[Go to docs](https://svelte-cssgg-icons.vercel.app)
## Props
@prop export let size = ctx.size || '24';
@prop export let role = ctx.role || 'img';
@prop export let color = ctx.color || 'currentColor';
@prop export let ariaLabel = 'volume';
-->
