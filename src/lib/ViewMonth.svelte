<script>
  import { getContext } from 'svelte';
  const ctx = getContext('iconCtx') ?? {};
  export let size = ctx.size || '24';
  export let role = ctx.role || 'img';
  export let color = ctx.color || 'currentColor';
  export let ariaLabel = 'view month';
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
    d="M2 8C2 6.34315 3.34315 5 5 5H19C20.6569 5 22 6.34315 22 8V16C22 17.6569 20.6569 19 19 19H5C3.34315 19 2 17.6569 2 16V8ZM17 7H19C19.5523 7 20 7.44771 20 8V9H17V7ZM15 7H13V9H15V7ZM11 7H9V9H11V7ZM7 7H5C4.44772 7 4 7.44772 4 8V9H7V7ZM4 11V13H7V11H4ZM4 15V16C4 16.5523 4.44772 17 5 17H7V15H4ZM9 17H11V15H9V17ZM13 17H15V15H13V17ZM17 17H19C19.5523 17 20 16.5523 20 16V15H17V17ZM20 13V11H17V13H20ZM11 13H9V11H11V13ZM15 13H13V11H15V13Z"
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
@prop export let ariaLabel = 'view month';
-->
