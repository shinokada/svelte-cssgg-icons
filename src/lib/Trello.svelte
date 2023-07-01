<script>
  export let color = 'currentColor';
  export let size = '24';
  export let role = 'img';
  export let ariaLabel = 'trello';
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
    d="M6 7C6 6.44771 6.44772 6 7 6H10C10.5523 6 11 6.44772 11 7V17C11 17.5523 10.5523 18 10 18H7C6.44772 18 6 17.5523 6 17V7Z"
    fill={color}
  />
  <path
    d="M13 7C13 6.44772 13.4477 6 14 6H17C17.5523 6 18 6.44772 18 7V13C18 13.5523 17.5523 14 17 14H14C13.4477 14 13 13.5523 13 13V7Z"
    fill={color}
  />
  <path
    fill-rule="evenodd"
    clip-rule="evenodd"
    d="M2 4C2 2.89543 2.89543 2 4 2H20C21.1046 2 22 2.89543 22 4V20C22 21.1046 21.1046 22 20 22H4C2.89543 22 2 21.1046 2 20V4ZM4 4H20V20H4V4Z"
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
