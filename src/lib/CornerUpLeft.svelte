<script>
  import { getContext } from 'svelte';
  const ctx = getContext('iconCtx') ?? {};
  export let size = ctx.size || '24';
  export let role = ctx.role || 'img';
  export let color = ctx.color || 'currentColor';
  export let ariaLabel = 'corner up left';
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
    d="M10.6276 14.7219L9.21641 16.1391L2.83875 9.78892L9.18897 3.41125L10.6062 4.82242L6.82971 8.61526L17.1353 8.59304C19.3445 8.58828 21.1392 10.3753 21.144 12.5844L21.1612 20.5844L19.1612 20.5887L19.144 12.5887C19.1416 11.4841 18.2442 10.5907 17.1396 10.593L6.50391 10.616L10.6276 14.7219Z"
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
@prop export let ariaLabel = 'corner up left';
-->
