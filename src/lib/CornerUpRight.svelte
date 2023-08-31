<script>
  export let color = 'currentColor';
  export let size = '24';
  export let role = 'img';
  export let ariaLabel = 'corner up right';
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
    d="M13.3724 14.7219L14.7835 16.1391L21.1612 9.78892L14.811 3.41125L13.3937 4.82242L17.1702 8.61526L6.86461 8.59304C4.65547 8.58828 2.86076 10.3753 2.85599 12.5844L2.83875 20.5844L4.83874 20.5887L4.85599 12.5887C4.85837 11.4841 5.75573 10.5907 6.8603 10.593L17.496 10.616L13.3724 14.7219Z"
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
@prop export let ariaLabel = 'corner up right';
-->
