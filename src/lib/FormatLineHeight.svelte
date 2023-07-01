<script>
  export let color = 'currentColor';
  export let size = '24';
  export let role = 'img';
  export let ariaLabel = 'format line height';
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
    d="M5.09668 6.99707H7.17358L4.17358 3.99707L1.17358 6.99707H3.09668V17.0031H1.15881L4.15881 20.0031L7.15881 17.0031H5.09668V6.99707Z"
    fill={color}
  />
  <path d="M22.8412 7H8.84119V5H22.8412V7Z" fill={color} />
  <path d="M22.8412 11H8.84119V9H22.8412V11Z" fill={color} />
  <path d="M8.84119 15H22.8412V13H8.84119V15Z" fill={color} />
  <path d="M22.8412 19H8.84119V17H22.8412V19Z" fill={color} />
</svg>
<!--
@component
[Go to Document](https://shinokada.github.io/svelte-cssgg-icons/)
## Props
@prop role = 'img';
@prop size = '24';
@prop color = 'currentColor'
@prop ariaLabel='file name'
## Event
- on:click
- on:keydown
- on:keyup
- on:focus
- on:blur
- on:mouseenter
- on:mouseleave
- on:mouseover
- on:mouseout
-->
