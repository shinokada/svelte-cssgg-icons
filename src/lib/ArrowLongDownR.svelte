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
    d="M16.2416 4.64146L11.9989 0.398819L7.75629 4.64146L11.0003 7.88551L11.013 19.7865L9.16846 17.9523L7.75821 19.3704L12.0127 23.6012L16.2437 19.3466L14.8255 17.9363L13.013 19.7591L13.0003 7.8827L16.2416 4.64146ZM10.5847 4.64146L11.9989 3.22725L13.4131 4.64146L11.9989 6.05567L10.5847 4.64146Z"
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
