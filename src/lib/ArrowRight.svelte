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
    d="M15.0378 6.34317L13.6269 7.76069L16.8972 11.0157L3.29211 11.0293L3.29413 13.0293L16.8619 13.0157L13.6467 16.2459L15.0643 17.6568L20.7079 11.9868L15.0378 6.34317Z"
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
