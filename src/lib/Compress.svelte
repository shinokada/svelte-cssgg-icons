<script>
  import { getContext } from 'svelte';
  const ctx = getContext('iconCtx') ?? {};
  export let size = ctx.size || '24';
  export let role = ctx.role || 'img';
  export let color = ctx.color || 'currentColor';
  export let ariaLabel = 'compress';
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
    d="M19.0954 8.42986L17.6711 7.02576L12.7568 12.0107L17.7417 16.925L19.1458 15.5007L16.644 13.0344L23.1411 13.0847L23.1565 11.0848L16.5286 11.0334L19.0954 8.42986Z"
    fill={color}
  />
  <path
    d="M5.46742 15.5618L6.88341 16.9742L11.827 12.0183L6.87102 7.07476L5.45857 8.49074L8.04995 11.0756L0.843506 11.1004L0.850384 13.1004L7.94701 13.076L5.46742 15.5618Z"
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
@prop export let ariaLabel = 'compress';
-->
