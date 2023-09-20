<script>
  import { getContext } from 'svelte';
  const ctx = getContext('iconCtx') ?? {};
  export let size = ctx.size || '24';
  export let role = ctx.role || 'img';
  export let color = ctx.color || 'currentColor';
  export let ariaLabel = 'corner right up';
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
    d="M9.28999 10.6254L7.87709 9.20989L14.2469 2.85181L20.605 9.22164L19.1895 10.6346L15.4082 6.84631L15.3987 17.152C15.3967 19.3611 13.6042 21.1503 11.395 21.1483L3.39502 21.1409L3.39687 19.1409L11.3969 19.1483C12.5014 19.1493 13.3977 18.2547 13.3987 17.1501L13.4085 6.51446L9.28999 10.6254Z"
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
@prop export let ariaLabel = 'corner right up';
-->
