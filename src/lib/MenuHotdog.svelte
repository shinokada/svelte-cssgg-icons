<script>
  export let color = 'currentColor';
  export let size = '24';
  export let role = 'img';
  export let ariaLabel = 'menu hotdog';
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
  <path d="M7 6C5.34315 6 4 7.34315 4 9H20C20 7.34315 18.6569 6 17 6H7Z" fill={color} />
  <path d="M7 18C5.34315 18 4 16.6569 4 15H20C20 16.6569 18.6569 18 17 18H7Z" fill={color} />
  <path
    d="M3 11C2.44772 11 2 11.4477 2 12C2 12.5523 2.44772 13 3 13H21C21.5523 13 22 12.5523 22 12C22 11.4477 21.5523 11 21 11H3Z"
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
