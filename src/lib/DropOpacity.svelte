<script>
  import { getContext } from 'svelte';
  const ctx = getContext('iconCtx') ?? {};
  export let size = ctx.size || '24';
  export let role = ctx.role || 'img';
  export let color = ctx.color || 'currentColor';
  export let ariaLabel = 'drop opacity';
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
    d="M15.9451 21.9559C12.5884 23.5927 8.42477 23.0167 5.63598 20.2279C2.12126 16.7132 2.12126 11.0147 5.63598 7.49995L11.9999 1.13599L18.3639 7.49995C19.2521 8.38814 19.9158 9.41578 20.3551 10.5124C21.6543 13.7553 20.9906 17.6012 18.364 20.2278C17.6381 20.9538 16.8189 21.5298 15.9451 21.9559ZM7.05019 8.91416L11.9999 3.96441L16.9497 8.91416C18.274 10.2385 18.9568 11.9615 18.998 13.6968H5.00192C5.04309 11.9615 5.72585 10.2385 7.05019 8.91416Z"
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
@prop export let ariaLabel = 'drop opacity';
-->
