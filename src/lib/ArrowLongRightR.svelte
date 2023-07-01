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
    d="M19.3514 7.72525L23.6012 11.9607L19.3655 16.2105L17.9489 14.7987L19.7633 12.9781L7.89744 13.0188L4.64151 16.2748L0.398865 12.0321L4.64151 7.78947L7.87093 11.0189L19.782 10.9781L17.9395 9.14185L19.3514 7.72525ZM4.64151 13.4463L6.05572 12.0321L4.64151 10.6179L3.22729 12.0321L4.64151 13.4463Z"
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
