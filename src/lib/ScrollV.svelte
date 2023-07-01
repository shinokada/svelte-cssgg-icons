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
    d="M9.17154 16.8182L7.75732 18.2324L12 22.475L16.2426 18.2324L14.8284 16.8182L12 19.6466L9.17154 16.8182Z"
    fill="{color}"
  />
  <path
    d="M14.8284 7.182L16.2426 5.76779L12 1.52515L7.75733 5.76779L9.17155 7.182L12 4.35357L14.8284 7.182Z"
    fill="{color}"
  />
  <path
    fill-rule="evenodd"
    clip-rule="evenodd"
    d="M12 9.00018C13.6569 9.00018 15 10.3433 15 12.0002C15 13.657 13.6569 15.0002 12 15.0002C10.3431 15.0002 9 13.657 9 12.0002C9 10.3433 10.3431 9.00018 12 9.00018ZM12 11.0002C12.5523 11.0002 13 11.4479 13 12.0002C13 12.5525 12.5523 13.0002 12 13.0002C11.4477 13.0002 11 12.5525 11 12.0002C11 11.4479 11.4477 11.0002 12 11.0002Z"
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
