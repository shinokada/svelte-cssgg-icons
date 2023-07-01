<script>
  export let color = 'currentColor';
  export let size = '24';
  export let role = 'img';
  export let ariaLabel = 'board';
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
    d="M6 4C3.79086 4 2 5.79086 2 8V16C2 18.2091 3.79086 20 6 20H18C20.2091 20 22 18.2091 22 16V8C22 5.79086 20.2091 4 18 4H6ZM14 6H10V18H14V6ZM16 6V18H18C19.1046 18 20 17.1046 20 16V8C20 6.89543 19.1046 6 18 6H16ZM6 18H8V6H6C4.89543 6 4 6.89543 4 8V16C4 17.1046 4.89543 18 6 18Z"
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
