<script>
  import { getContext } from 'svelte';
  const ctx = getContext('iconCtx') ?? {};
  export let size = ctx.size || '24';
  export let role = ctx.role || 'img';
  export let color = ctx.color || 'currentColor';
  export let ariaLabel = 'arrow long up r';
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
    d="M7.79337 4.60945L12.0679 0.398956L16.2785 4.67358L14.8536 6.07708L13.0499 4.24596L12.9809 16.1324L16.2068 19.3584L11.9642 23.601L7.72156 19.3584L10.981 16.0989L11.0501 4.20883L9.19686 6.0343L7.79337 4.60945ZM11.9642 20.7726L13.3784 19.3584L11.9642 17.9442L10.55 19.3584L11.9642 20.7726Z"
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
@prop export let ariaLabel = 'arrow long up r';
-->
