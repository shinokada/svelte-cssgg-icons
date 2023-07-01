<script>
  export let color = 'currentColor';
  export let size = '24';
  export let role = 'img';
  export let ariaLabel = 'glass alt';
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
    d="M5 2H19L17.3602 18.398C17.1557 20.4428 15.4351 22 13.38 22H10.62C8.56494 22 6.84428 20.4428 6.6398 18.398L5 2ZM7.50998 7L7.20998 4H16.79L16.49 7H7.50998ZM7.70998 9L8.62988 18.199C8.73212 19.2214 9.59245 20 10.62 20H13.38C14.4076 20 15.2679 19.2214 15.3701 18.199L16.29 9H7.70998Z"
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
