<script>
  export let color = 'currentColor';
  export let size = '24';
  export let role = 'img';
  export let ariaLabel = 'arrow long left e';
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
    d="M5.26323 7.75737L1.01343 11.9928L5.24893 16.2426L6.66553 14.8308L4.85123 13.0104L16.9685 13.0519L16.9596 15.0507L22.9595 15.0777L22.9865 9.07773L16.9865 9.05079L16.9775 11.0519L4.83252 11.0103L6.67505 9.17397L5.26323 7.75737ZM20.9775 11.0687L20.9685 13.0687L18.9685 13.0597L18.9775 11.0597L20.9775 11.0687Z"
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
@prop export let ariaLabel = 'arrow long left e';
-->
