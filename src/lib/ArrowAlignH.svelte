<script>
 export let color = "currentColor"
 export let size="24";
 export let role="img";
</script>
<svg
  width="{size}"
  height="{size}"
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
  <path d="M13 7H11V17H13V7Z" fill="{color}" />
  <path
    d="M5.99996 7.75732L7.41418 9.17154L5.58572 11L9.99996 11V13L5.58579 13L7.41418 14.8284L5.99996 16.2426L1.75732 12L5.99996 7.75732Z"
    fill="{color}"
  />
  <path
    d="M18 16.2427L16.5858 14.8285L18.4143 13H14V11L18.4142 11L16.5858 9.17161L18 7.75739L22.2427 12L18 16.2427Z"
    fill="{color}"
  />
</svg>
<!--
@component
[Go to Document](https://shinokada.github.io/svelte-supertiny/)
## Props
@prop role = img;
@prop size = '24';
@prop color = 'currentColor'
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
