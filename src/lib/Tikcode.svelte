<script>
  export let color = 'currentColor';
  export let size = '24';
  export let role = 'img';
  export let ariaLabel = 'tikcode';
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
  <path fill-rule="evenodd" clip-rule="evenodd" d="M9 5H5V9H9V5ZM3 3V11H11V3H3Z" fill={color} />
  <path
    fill-rule="evenodd"
    clip-rule="evenodd"
    d="M19 5H15V9H19V5ZM13 3V11H21V3H13Z"
    fill={color}
  />
  <path
    fill-rule="evenodd"
    clip-rule="evenodd"
    d="M9 15H5V19H9V15ZM3 13V21H11V13H3Z"
    fill={color}
  />
  <path d="M13 13H15V21H13V13Z" fill={color} />
  <path d="M16 13H18V21H16V13Z" fill={color} />
  <path d="M19 13H21V21H19V13Z" fill={color} />
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
