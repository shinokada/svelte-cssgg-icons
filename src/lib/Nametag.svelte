<script>
  import { getContext } from 'svelte';
  const ctx = getContext('iconCtx') ?? {};
  export let size = ctx.size || '24';
  export let role = ctx.role || 'img';
  export let color = ctx.color || 'currentColor';
  export let ariaLabel = 'nametag';
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
  <path d="M4 14V20H10V18H6V14H4Z" fill={color} />
  <path
    fill-rule="evenodd"
    clip-rule="evenodd"
    d="M9 9V15H15V9H9ZM13 11H11V13H13V11Z"
    fill={color}
  />
  <path d="M4 10V4H10V6H6V10H4Z" fill={color} />
  <path d="M20 10V4H14V6H18V10H20Z" fill={color} />
  <path d="M20 14V20H14V18H18V14H20Z" fill={color} />
</svg>

<!--
@component
[Go to docs](https://svelte-cssgg-icons.vercel.app)
## Props
@prop export let size = ctx.size || '24';
@prop export let role = ctx.role || 'img';
@prop export let color = ctx.color || 'currentColor';
@prop export let ariaLabel = 'nametag';
-->
