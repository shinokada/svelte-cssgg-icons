<script>
  import { getContext } from 'svelte';
  const ctx = getContext('iconCtx') ?? {};
  export let size = ctx.size || '24';
  export let role = ctx.role || 'img';
  export let color = ctx.color || 'currentColor';
  export let ariaLabel = 'google tasks';
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
    d="M16.7679 5.71447C17.4779 4.86832 18.7394 4.75795 19.5856 5.46796C20.4317 6.17796 20.5421 7.43947 19.8321 8.28562L10.833 19.0102C10.123 19.8564 8.86153 19.9668 8.01538 19.2568C7.16923 18.5468 7.05886 17.2852 7.76886 16.4391L16.7679 5.71447Z"
    fill={color}
  />
  <path
    d="M3 12.7396C3 11.6351 3.89543 10.7396 5 10.7396C6.10457 10.7396 7 11.6351 7 12.7396C7 13.8442 6.10457 14.7396 5 14.7396C3.89543 14.7396 3 13.8442 3 12.7396Z"
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
@prop export let ariaLabel = 'google tasks';
-->
