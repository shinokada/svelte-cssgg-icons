<script>
  import { getContext } from 'svelte';
  const ctx = getContext('iconCtx') ?? {};
  export let size = ctx.size || '24';
  export let role = ctx.role || 'img';
  export let color = ctx.color || 'currentColor';
  export let ariaLabel = 'calculator';
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
  <path d="M17 5H7V7H17V5Z" fill={color} />
  <path d="M7 9H9V11H7V9Z" fill={color} />
  <path d="M9 13H7V15H9V13Z" fill={color} />
  <path d="M7 17H9V19H7V17Z" fill={color} />
  <path d="M13 9H11V11H13V9Z" fill={color} />
  <path d="M11 13H13V15H11V13Z" fill={color} />
  <path d="M13 17H11V19H13V17Z" fill={color} />
  <path d="M15 9H17V11H15V9Z" fill={color} />
  <path d="M17 13H15V19H17V13Z" fill={color} />
  <path
    fill-rule="evenodd"
    clip-rule="evenodd"
    d="M3 3C3 1.89543 3.89543 1 5 1H19C20.1046 1 21 1.89543 21 3V21C21 22.1046 20.1046 23 19 23H5C3.89543 23 3 22.1046 3 21V3ZM5 3H19V21H5V3Z"
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
@prop export let ariaLabel = 'calculator';
-->
