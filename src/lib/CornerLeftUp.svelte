<script>
  import { getContext } from 'svelte';
  const ctx = getContext('iconCtx') ?? {};
  export let size = ctx.size || '24';
  export let role = ctx.role || 'img';
  export let color = ctx.color || 'currentColor';
  export let ariaLabel = 'corner left up';
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
    d="M14.71 10.6254L16.1229 9.20989L9.7531 2.85181L3.39502 9.22164L4.81054 10.6346L8.59179 6.84631L8.60131 17.152C8.60335 19.3611 10.3959 21.1503 12.605 21.1483L20.605 21.1409L20.6032 19.1409L12.6032 19.1483C11.4986 19.1493 10.6023 18.2547 10.6013 17.1501L10.5915 6.51446L14.71 10.6254Z"
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
@prop export let ariaLabel = 'corner left up';
-->
