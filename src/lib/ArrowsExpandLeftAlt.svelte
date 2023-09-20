<script>
  import { getContext } from 'svelte';
  const ctx = getContext('iconCtx') ?? {};
  export let size = ctx.size || '24';
  export let role = ctx.role || 'img';
  export let color = ctx.color || 'currentColor';
  export let ariaLabel = 'arrows expand left alt';
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
    d="M10.1005 2.10052V4.10052H5.51471L11.293 9.87878L9.87875 11.293L4.10046 5.51471L4.10046 10.1005H2.10046L2.10046 2.10052H10.1005Z"
    fill={color}
  />
  <path
    d="M21.8995 13.8995H19.8995V18.4853L14.1212 12.707L12.707 14.1213L18.4853 19.8995H13.8995V21.8995H21.8995V13.8995Z"
    fill={color}
  />
  <path
    d="M16.2426 9.1716L14.8284 7.75739L7.7573 14.8285L9.17151 16.2427L16.2426 9.1716Z"
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
@prop export let ariaLabel = 'arrows expand left alt';
-->
