<script>
  export let color = 'currentColor';
  export let size = '24';
  export let role = 'img';
  export let ariaLabel = 'screen wide';
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
    d="M11 16H3C1.34315 16 0 14.6569 0 13V8C0 6.34315 1.34315 5 3 5H21C22.6569 5 24 6.34315 24 8V13C24 14.6569 22.6569 16 21 16H13V17H15C15.5523 17 16 17.4477 16 18C16 18.5523 15.5523 19 15 19H9C8.44771 19 8 18.5523 8 18C8 17.4477 8.44771 17 9 17H11V16ZM3 7H21C21.5523 7 22 7.44772 22 8V13C22 13.5523 21.5523 14 21 14H3C2.44772 14 2 13.5523 2 13V8C2 7.44772 2.44772 7 3 7Z"
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
@prop export let ariaLabel = 'screen wide';
-->
