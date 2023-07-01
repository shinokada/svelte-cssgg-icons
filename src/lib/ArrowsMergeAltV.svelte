<script>
  export let color = 'currentColor';
  export let size = '24';
  export let role = 'img';
  export let ariaLabel = 'arrows merge alt v';
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
    d="M18 1.5033V3.5033L13 3.5033V7.6749L14.8285 5.84644L16.2427 7.26066L12 11.5033L7.75739 7.26066L9.17161 5.84644L11 7.67483V3.5033L6 3.5033V1.5033L18 1.5033Z"
    fill={color}
  />
  <path
    d="M18 20.4967V22.4967H6V20.4967H11V16.3251L9.17154 18.1536L7.75732 16.7393L12 12.4967L16.2426 16.7393L14.8284 18.1536L13 16.3252V20.4967H18Z"
    fill={color}
  />
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
