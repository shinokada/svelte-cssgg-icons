<script>
  export let color = 'currentColor';
  export let size = '24';
  export let role = 'img';
  export let ariaLabel = 'format bold';
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
    d="M11 4.504H7v14.992h6a4 4 0 0 0 .604-7.955A4 4 0 0 0 11 4.505Zm-2 2h2a2 2 0 1 1 0 4H9v-4Zm0 10.991v-4h4a2 2 0 1 1 0 4H9Z"
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
