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
    d="M15.3052 12L18.1299 9.17526L16.7157 7.76105L13.891 10.5858L13.8873 10.5821L12.4731 11.9963L12.4768 12L12.4731 12.0037L13.8873 13.4179L13.891 13.4142L16.7157 16.239L18.1299 14.8248L15.3052 12Z"
    fill="{color}"
  />
  <path
    d="M10.1091 10.5858L10.1128 10.5821L11.527 11.9963L11.5233 12L11.527 12.0037L10.1128 13.4179L10.1091 13.4142L7.28433 16.239L5.87012 14.8248L8.69487 12L5.87012 9.17526L7.28433 7.76105L10.1091 10.5858Z"
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
