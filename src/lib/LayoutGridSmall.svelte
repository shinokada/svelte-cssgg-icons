<script>
  import { getContext } from 'svelte';
  const ctx = getContext('iconCtx') ?? {};
  export let size = ctx.size || '24';
  export let role = ctx.role || 'img';
  export let color = ctx.color || 'currentColor';
  export let ariaLabel = 'layout grid small';
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
  <path d="M7 7H9V9H7V7Z" fill={color} />
  <path d="M11 7H13V9H11V7Z" fill={color} />
  <path d="M17 7H15V9H17V7Z" fill={color} />
  <path d="M7 11H9V13H7V11Z" fill={color} />
  <path d="M13 11H11V13H13V11Z" fill={color} />
  <path d="M15 11H17V13H15V11Z" fill={color} />
  <path d="M9 15H7V17H9V15Z" fill={color} />
  <path d="M11 15H13V17H11V15Z" fill={color} />
  <path d="M17 15H15V17H17V15Z" fill={color} />
</svg>

<!--
@component
[Go to docs](https://svelte-cssgg-icons.vercel.app)
## Props
@prop export let size = ctx.size || '24';
@prop export let role = ctx.role || 'img';
@prop export let color = ctx.color || 'currentColor';
@prop export let ariaLabel = 'layout grid small';
-->
