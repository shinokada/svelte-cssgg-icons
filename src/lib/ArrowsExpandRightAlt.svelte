<script>
  import { getContext } from 'svelte';
  const ctx = getContext('iconCtx') ?? {};
  export let size = ctx.size || '24';
  export let role = ctx.role || 'img';
  export let color = ctx.color || 'currentColor';
  export let ariaLabel = 'arrows expand right alt';
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
    d="M13.8995 2.10052V4.10052H18.4852L12.707 9.87878L14.1212 11.293L19.8995 5.51471V10.1005H21.8995V2.10052H13.8995Z"
    fill={color}
  />
  <path
    d="M5.51468 19.8995H10.1005V21.8995H2.10046V13.8995H4.10046V18.4853L9.87872 12.707L11.2929 14.1213L5.51468 19.8995Z"
    fill={color}
  />
  <path
    d="M9.17154 7.75739L7.75732 9.1716L14.8284 16.2427L16.2426 14.8285L9.17154 7.75739Z"
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
@prop export let ariaLabel = 'arrows expand right alt';
-->
