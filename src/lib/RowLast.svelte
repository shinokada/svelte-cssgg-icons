<script>
  export let color = 'currentColor';
  export let size = '24';
  export let role = 'img';
  export let ariaLabel = 'row last';
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
  <g opacity="0.5">
    <path
      d="M6 13C5.44772 13 5 12.5523 5 12C5 11.4477 5.44772 11 6 11H14C14.5523 11 15 11.4477 15 12C15 12.5523 14.5523 13 14 13H6Z"
      fill={color}
    />
    <path
      d="M6 9C5.44772 9 5 8.55228 5 8C5 7.44772 5.44772 7 6 7H14C14.5523 7 15 7.44772 15 8C15 8.55228 14.5523 9 14 9H6Z"
      fill={color}
    />
  </g>
  <path
    d="M5 16C5 16.5523 5.44772 17 6 17H18C18.5523 17 19 16.5523 19 16C19 15.4477 18.5523 15 18 15H6C5.44772 15 5 15.4477 5 16Z"
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
@prop export let ariaLabel = 'row last';
-->
