<script>
  export let color = 'currentColor';
  export let size = '24';
  export let role = 'img';
  export let ariaLabel = 'chevron double down';
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
    d="M7.75735 5.63605L6.34314 7.05026L12 12.7071L17.6569 7.05029L16.2427 5.63608L12 9.87872L7.75735 5.63605Z"
    fill={color}
  />
  <path
    d="M6.34314 12.7071L7.75735 11.2929L12 15.5356L16.2427 11.2929L17.6569 12.7071L12 18.364L6.34314 12.7071Z"
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
