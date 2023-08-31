<script>
  export let color = 'currentColor';
  export let size = '24';
  export let role = 'img';
  export let ariaLabel = 'inbox';
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
    d="M2 5C2 3.34315 3.34315 2 5 2H19C20.6569 2 22 3.34315 22 5V20C22 21.1046 21.1046 22 20 22H8.1477C8.09893 22.0036 8.04968 22.0054 8 22.0054H4C2.89543 22.0054 2 21.1099 2 20.0054V5ZM5 4H19C19.5523 4 20 4.44771 20 5V14H16C14.8954 14 14 14.8954 14 16V17H10V16.0054C10 14.9008 9.10457 14.0054 8 14.0054H4V5C4 4.44772 4.44771 4 5 4Z"
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
@prop export let ariaLabel = 'inbox';
-->
