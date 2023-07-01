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
  <path d="M3 4H15V8H3V4Z" fill="{color}" />
  <path d="M21 8H17V4H21V8Z" fill="{color}" />
  <path d="M3 10H21V14H3V10Z" fill="{color}" />
  <path d="M11 16H3V20H11V16Z" fill="{color}" />
  <path d="M13 16V20H21V16H13Z" fill="{color}" />
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
