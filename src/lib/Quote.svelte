<script>
  export let color = 'currentColor';
  export let size = '24';
  export let role = 'img';
  export let ariaLabel = 'quote';
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
  <path d="M9.13456 9H12.1346L10 14.6075H7L9.13456 9Z" fill={color} />
  <path d="M14.1346 9H17.1346L15 14.6075H12L14.1346 9Z" fill={color} />
</svg>

<!--
@component
[Go to docs](https://svelte-cssgg-icons.vercel.app)
## Props
@prop export let color = 'currentColor';
@prop export let size = '24';
@prop export let role = 'img';
@prop export let ariaLabel = 'quote';
-->
