<script>
  export let color = 'currentColor';
  export let size = '24';
  export let role = 'img';
  export let ariaLabel = 'maximize';
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
  <path d="M3 3H9V5H5V9H3V3Z" fill={color} />
  <path d="M3 21H9V19H5V15H3V21Z" fill={color} />
  <path d="M15 21H21V15H19V19H15V21Z" fill={color} />
  <path d="M21 3H15V5H19V9H21V3Z" fill={color} />
</svg>

<!--
@component
[Go to docs](https://svelte-cssgg-icons.vercel.app)
## Props
@prop export let color = 'currentColor';
@prop export let size = '24';
@prop export let role = 'img';
@prop export let ariaLabel = 'maximize';
-->
