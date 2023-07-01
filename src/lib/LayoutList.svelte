<script>
  export let color = 'currentColor';
  export let size = '24';
  export let role = 'img';
  export let ariaLabel = 'layout list';
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
  <path d="M9 7H7V9H9V7Z" fill={color} />
  <path d="M7 13V11H9V13H7Z" fill={color} />
  <path d="M7 15V17H9V15H7Z" fill={color} />
  <path d="M11 15V17H17V15H11Z" fill={color} />
  <path d="M17 13V11H11V13H17Z" fill={color} />
  <path d="M17 7V9H11V7H17Z" fill={color} />
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
