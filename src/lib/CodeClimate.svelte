<script>
  export let color = 'currentColor';
  export let size = '24';
  export let role = 'img';
  export let ariaLabel = 'code climate';
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
    d="M9.49506 8.1109L3.1311 14.4749L4.54532 15.8891L9.49506 10.9393L14.4448 15.8891L15.859 14.4749L9.49506 8.1109Z"
    fill={color}
  />
  <path
    d="M14.5049 8.11092L12.5317 10.0842L13.9503 11.494L14.5049 10.9393L19.4547 15.8891L20.8689 14.4749L14.5049 8.11092Z"
    fill={color}
  />
</svg>

<!--
@component
[Go to docs](https://svelte-cssgg-icons.vercel.app)
## Props
@prop export let color = 'currentColor';
@prop export let size = '24';
@prop export let role = 'img';
@prop export let ariaLabel = 'code climate';
-->
