<script>
  export let color = 'currentColor';
  export let size = '24';
  export let role = 'img';
  export let ariaLabel = 'display spacing';
</script>

<svg
  width={size}
  height={size}
  {role}
  {...$$restProps}
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
  <path d="M3 21V3H5V21H3Z" fill={color} />
  <path fill-rule="evenodd" clip-rule="evenodd" d="M7 3H17V21H7V3ZM9 5V19H15V5H9Z" fill={color} />
  <path d="M19 3V21H21V3H19Z" fill={color} />
</svg>
<!--
@component
[Go to Document](https://shinokada.github.io/svelte-supertiny/)
## Props
@prop role = img;
@prop size = '24';
@prop color = 'currentColor'
@prop ariaLabel=file name
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
