<script>
  export let color = 'currentColor';
  export let size = '24';
  export let role = 'img';
  export let ariaLabel = 'arrows breake h';
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
    d="M9.24268 7H11.2427V11.0001H11.2477V13.0001H11.2427V17H9.24268V13.0001L4.82846 13L6.65685 14.8284L5.24264 16.2426L1 12L5.24264 7.75732L6.65685 9.17154L4.82839 11H9.24264L9.24268 7Z"
    fill={color}
  />
  <path
    d="M15.2527 7.00012H13.2527V11.0001H13.2477V13.0001H13.2527V17.0001H15.2527V13.0001L19.667 13L17.8385 14.8285L19.2527 16.2427L23.4954 12L19.2527 7.75739L17.8385 9.17161L19.6669 11H15.2527L15.2527 7.00012Z"
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
@prop export let ariaLabel = 'arrows breake h';
-->
