<script>
  export let color = 'currentColor';
  export let size = '24';
  export let role = 'img';
  export let ariaLabel = 'path outline';
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
    d="M5 5H15V9H19V19H9V15H5V5ZM7 7H13V9H9V13H7V7ZM11 17H17V11H15V15H11V17ZM13 11H11V13H13V11Z"
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
@prop export let ariaLabel = 'path outline';
-->
