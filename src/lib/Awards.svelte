<script>
  export let color = 'currentColor';
  export let size = '24';
  export let role = 'img';
  export let ariaLabel = 'awards';
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
    d="M19 9C19 11.3787 17.8135 13.4804 16 14.7453V22H13.4142L12 20.5858L10.5858 22H8V14.7453C6.18652 13.4804 5 11.3787 5 9C5 5.13401 8.13401 2 12 2C15.866 2 19 5.13401 19 9ZM17 9C17 11.7614 14.7614 14 12 14C9.23858 14 7 11.7614 7 9C7 6.23858 9.23858 4 12 4C14.7614 4 17 6.23858 17 9ZM10 19.7573L12 17.7573L14 19.7574V15.7101C13.3663 15.8987 12.695 16 12 16C11.305 16 10.6337 15.8987 10 15.7101V19.7573Z"
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
@prop export let ariaLabel = 'awards';
-->
