<script>
  export let color = 'currentColor';
  export let size = '24';
  export let role = 'img';
  export let ariaLabel = 'ghost character';
</script>

<svg
  width={size}
  height={size}
  {role}
  {...$$restProps}
  aria-label={ariaLabel}
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
    d="M10.9759 9C10.9759 9.55228 10.5282 10 9.97589 10C9.42361 10 8.97589 9.55228 8.97589 9C8.97589 8.44771 9.42361 8 9.97589 8C10.5282 8 10.9759 8.44771 10.9759 9Z"
    fill={color}
  />
  <path
    d="M13.9712 10C14.5235 10 14.9712 9.55228 14.9712 9C14.9712 8.44771 14.5235 8 13.9712 8C13.4189 8 12.9712 8.44771 12.9712 9C12.9712 9.55228 13.4189 10 13.9712 10Z"
    fill={color}
  />
  <path
    fill-rule="evenodd"
    clip-rule="evenodd"
    d="M19 20.9999V10C19 6.13401 15.866 3 12 3C8.13401 3 5 6.13401 5 10V21L7.82846 21L9.24264 19.5858L10.6569 21L13.3433 21L14.7574 19.5858L16.1717 21L19 20.9999ZM17 10C17 7.23858 14.7614 5 12 5C9.23858 5 7 7.23858 7 10V19L9.24264 16.7573L12 19.5147L14.7574 16.7573L17 18.9999V10Z"
    fill={color}
  />
</svg>
<!--
@component
[Go to Document](https://shinokada.github.io/svelte-cssgg-icons/)
## Props
@prop role = 'img';
@prop size = '24';
@prop color = 'currentColor'
@prop ariaLabel='file name'
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
