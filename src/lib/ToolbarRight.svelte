<script>
  export let color = 'currentColor';
  export let size = '24';
  export let role = 'img';
  export let ariaLabel = 'toolbar right';
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
  <path d="M16 9H18V15H16V9Z" fill={color} />
  <path
    fill-rule="evenodd"
    clip-rule="evenodd"
    d="M22 8C22 6.34315 20.6569 5 19 5H5C3.34315 5 2 6.34315 2 8V16C2 17.6569 3.34315 19 5 19H19C20.6569 19 22 17.6569 22 16V8ZM19 7H5C4.44772 7 4 7.44771 4 8V16C4 16.5523 4.44772 17 5 17H19C19.5523 17 20 16.5523 20 16V8C20 7.44772 19.5523 7 19 7Z"
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
