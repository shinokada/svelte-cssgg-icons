<script>
  import { getContext } from 'svelte';
  const ctx = getContext('iconCtx') ?? {};
  export let size = ctx.size || '24';
  export let role = ctx.role || 'img';
  export let color = ctx.color || 'currentColor';
  export let ariaLabel = 'toggle square off';
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
    d="M15 9C14.4477 9 14 9.44772 14 10V14C14 14.5523 14.4477 15 15 15H19C19.5523 15 20 14.5523 20 14V10C20 9.44772 19.5523 9 19 9H15Z"
    fill={color}
  />
  <path
    fill-rule="evenodd"
    clip-rule="evenodd"
    d="M0 7C0 5.89543 0.895431 5 2 5H22C23.1046 5 24 5.89543 24 7V17C24 18.1046 23.1046 19 22 19H2C0.89543 19 0 18.1046 0 17V7ZM2 7H22V17H2L2 7Z"
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
@prop export let ariaLabel = 'toggle square off';
-->
