<script>
  import { getContext } from 'svelte';
  const ctx = getContext('iconCtx') ?? {};
  export let size = ctx.size || '24';
  export let role = ctx.role || 'img';
  export let color = ctx.color || 'currentColor';
  export let ariaLabel = 'modem';
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
    d="M18 16.6341C18 17.1864 17.5523 17.6341 17 17.6341C16.4477 17.6341 16 17.1864 16 16.6341C16 16.0819 16.4477 15.6341 17 15.6341C17.5523 15.6341 18 16.0819 18 16.6341Z"
    fill={color}
  />
  <path
    fill-rule="evenodd"
    clip-rule="evenodd"
    d="M5.86603 3.13414C5.38773 2.858 4.77614 3.02187 4.5 3.50017C4.22386 3.97846 4.38773 4.59005 4.86603 4.86619L18.3205 12.6341H2V16.6341C2 18.8433 3.79086 20.6341 6 20.6341H18C20.2091 20.6341 22 18.8433 22 16.6341V12.6341L5.86603 3.13414ZM20 14.6341H4V16.6341C4 17.7387 4.89543 18.6341 6 18.6341H18C19.1046 18.6341 20 17.7387 20 16.6341V14.6341Z"
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
@prop export let ariaLabel = 'modem';
-->
