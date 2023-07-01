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
    d="M12 4C15.866 4 19 7.13401 19 11H5C5 7.13401 8.13401 4 12 4Z"
    fill="{color}"
  />
  <path d="M5 13H1V11H5V13Z" fill="{color}" />
  <path
    d="M19 13C19 16.866 15.866 20 12 20C8.13401 20 5 16.866 5 13H19Z"
    fill="{color}"
  />
  <path d="M19 13V11H23V13H19Z" fill="{color}" />
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
