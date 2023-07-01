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
  <path d="M11 8V10H8V14H11V16H6V8H11Z" fill="{color}" />
  <path d="M18 8V10H15V14H18V16H13V8H18Z" fill="{color}" />
  <path
    fill-rule="evenodd"
    clip-rule="evenodd"
    d="M2 5C2 4.44772 2.44772 4 3 4H21C21.5523 4 22 4.44772 22 5V19C22 19.5523 21.5523 20 21 20H3C2.44772 20 2 19.5523 2 19V5ZM4 18V6H20V18H4Z"
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
