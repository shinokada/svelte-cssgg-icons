<script>
  import { getContext } from 'svelte';
  const ctx = getContext('iconCtx') ?? {};
  export let size = ctx.size || '24';
  export let role = ctx.role || 'img';
  export let color = ctx.color || 'currentColor';
  export let ariaLabel = 'serverless';
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
  <path d="M11.7872 6H5V9H10.6953L11.7872 6Z" fill={color} />
  <path d="M9.96735 11H5V14H8.87544L9.96735 11Z" fill={color} />
  <path d="M11.0038 14L12.0957 11H20V14H11.0038Z" fill={color} />
  <path d="M8.1475 16H5V19H7.05559L8.1475 16Z" fill={color} />
  <path d="M9.18394 19L10.2759 16H20V19H9.18394Z" fill={color} />
  <path d="M12.8236 9L13.9156 6H20V9H12.8236Z" fill={color} />
</svg>

<!--
@component
[Go to docs](https://svelte-cssgg-icons.codewithshin.com)
## Props
@prop export let size = ctx.size || '24';
@prop export let role = ctx.role || 'img';
@prop export let color = ctx.color || 'currentColor';
@prop export let ariaLabel = 'serverless';
-->
