<script>
  export let color = 'currentColor';
  export let size = '24';
  export let role = 'img';
  export let ariaLabel = 'touchpad';
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
    d="M20 21C21.6569 21 23 19.6569 23 18V6C23 4.34315 21.6569 3 20 3H4C2.34315 3 1 4.34315 1 6V18C1 19.6569 2.34315 21 4 21H20ZM4 5H20C20.5523 5 21 5.44772 21 6V14H3V6C3 5.44772 3.44772 5 4 5ZM3 16V18C3 18.5523 3.44772 19 4 19H11V16H3ZM13 19V16H21V18C21 18.5523 20.5523 19 20 19H13Z"
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
@prop export let ariaLabel = 'touchpad';
-->
