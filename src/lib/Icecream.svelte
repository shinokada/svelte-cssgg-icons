<script>
  import { getContext } from 'svelte';
  const ctx = getContext('iconCtx') ?? {};
  export let size = ctx.size || '24';
  export let role = ctx.role || 'img';
  export let color = ctx.color || 'currentColor';
  export let ariaLabel = 'icecream';
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
    d="M15 17H19V8C19 4.13401 15.866 1 12 1C8.13401 1 5 4.13401 5 8V17H9V20C9 21.6569 10.3431 23 12 23C13.6569 23 15 21.6569 15 20V17ZM17 15V8C17 5.23858 14.7614 3 12 3C9.23858 3 7 5.23858 7 8V15H11V20C11 20.5523 11.4477 21 12 21C12.5523 21 13 20.5523 13 20V15H17Z"
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
@prop export let ariaLabel = 'icecream';
-->
