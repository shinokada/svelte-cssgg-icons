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
  <path d="M3 11H1V13H3V11Z" fill="{color}" />
  <path d="M7 11H5V13H7V11Z" fill="{color}" />
  <path d="M9 11H11V13H9V11Z" fill="{color}" />
  <path d="M15 11H13V13H15V11Z" fill="{color}" />
  <path d="M17 11H19V13H17V11Z" fill="{color}" />
  <path d="M23 11H21V13H23V11Z" fill="{color}" />
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
