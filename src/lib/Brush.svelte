<script>
  import { getContext } from 'svelte';
  const ctx = getContext('iconCtx') ?? {};
  export let size = ctx.size || '24';
  export let role = ctx.role || 'img';
  export let color = ctx.color || 'currentColor';
  export let ariaLabel = 'brush';
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
    d="M15 11H18C18.5523 11 19 11.4477 19 12V18C19 19.6569 17.6569 21 16 21H8C6.34315 21 5 19.6569 5 18V12C5 11.4477 5.44772 11 6 11H9V6C9 4.34315 10.3431 3 12 3C13.6569 3 15 4.34315 15 6V11ZM13 6C13 5.44772 12.5523 5 12 5C11.4477 5 11 5.44772 11 6V13H7V18C7 18.5523 7.44772 19 8 19H9V16H11V19H13V16H15V19H16C16.5523 19 17 18.5523 17 18V13H13V6Z"
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
@prop export let ariaLabel = 'brush';
-->
