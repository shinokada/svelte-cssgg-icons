<script>
  import { getContext } from 'svelte';
  const ctx = getContext('iconCtx') ?? {};
  export let size = ctx.size || '24';
  export let role = ctx.role || 'img';
  export let color = ctx.color || 'currentColor';
  export let ariaLabel = 'components';
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
    d="M7.7572 6.3431L11.9998 2.10046L16.2425 6.3431L11.9998 10.5857L7.7572 6.3431ZM10.5856 6.3431L11.9998 4.92889L13.4141 6.3431L11.9998 7.75732L10.5856 6.3431Z"
    fill={color}
  />
  <path
    fill-rule="evenodd"
    clip-rule="evenodd"
    d="M2.10046 11.9999L6.3431 7.75726L10.5857 11.9999L6.3431 16.2425L2.10046 11.9999ZM4.92889 11.9999L6.3431 10.5857L7.75732 11.9999L6.3431 13.4141L4.92889 11.9999Z"
    fill={color}
  />
  <path
    fill-rule="evenodd"
    clip-rule="evenodd"
    d="M13.4142 11.9999L17.6568 16.2425L21.8995 11.9999L17.6568 7.75726L13.4142 11.9999ZM17.6568 10.5857L16.2426 11.9999L17.6568 13.4141L19.071 11.9999L17.6568 10.5857Z"
    fill={color}
  />
  <path
    fill-rule="evenodd"
    clip-rule="evenodd"
    d="M7.7572 17.6569L11.9998 13.4142L16.2425 17.6569L11.9998 21.8995L7.7572 17.6569ZM10.5856 17.6569L11.9998 16.2427L13.4141 17.6569L11.9998 19.0711L10.5856 17.6569Z"
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
@prop export let ariaLabel = 'components';
-->
