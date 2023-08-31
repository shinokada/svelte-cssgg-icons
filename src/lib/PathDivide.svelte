<script>
  export let color = 'currentColor';
  export let size = '24';
  export let role = 'img';
  export let ariaLabel = 'path divide';
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
  <path d="M5 5H15V9H9V15H5V5Z" fill={color} />
  <path d="M9 15V19H19V9H15V15H9Z" fill={color} />
  <path d="M10 10H14V14H10V10Z" fill={color} />
</svg>

<!--
@component
[Go to docs](https://svelte-cssgg-icons.vercel.app)
## Props
@prop export let color = 'currentColor';
@prop export let size = '24';
@prop export let role = 'img';
@prop export let ariaLabel = 'path divide';
-->
