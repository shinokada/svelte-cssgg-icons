<script>
  import { getContext } from 'svelte';
  const ctx = getContext('iconCtx') ?? {};
  export let size = ctx.size || '24';
  export let role = ctx.role || 'img';
  export let color = ctx.color || 'currentColor';
  export let ariaLabel = 'corner double down left';
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
    d="M11.2952 7.69432L16.1357 2.6377L21.1924 7.47821L19.8094 8.92296L17.3474 6.56617L17.5094 12.6C17.5805 15.25 15.49 17.456 12.8399 17.5271L6.91369 17.6863L9.20765 19.9335L7.80805 21.3622L2.80768 16.4636L7.70628 11.4632L9.13495 12.8628L6.75759 15.2896L12.7755 15.128C14.1005 15.0924 15.1458 13.9895 15.1102 12.6645L14.9519 6.76668L12.74 9.07732L11.2952 7.69432Z"
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
@prop export let ariaLabel = 'corner double down left';
-->
