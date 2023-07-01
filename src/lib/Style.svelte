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
  <path
    fill-rule="evenodd"
    clip-rule="evenodd"
    d="M13 21V13H21V21H13ZM15 15H19L19 19H15V15Z"
    fill="{color}"
  />
  <path
    fill-rule="evenodd"
    clip-rule="evenodd"
    d="M3 11L3 3L11 3V11H3ZM5 5L9 5V9L5 9L5 5Z"
    fill="{color}"
  />
  <path d="M18 6V12H16V8L12 8V6L18 6Z" fill="{color}" />
  <path d="M12 18H6L6 12H8L8 16H12V18Z" fill="{color}" />
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
