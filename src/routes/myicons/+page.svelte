<script>
  import {Icon, icons} from '$lib';
  let size = "100";
  import { onMount } from 'svelte';
  const props = {
    name: 'arrow-down',
    size: '50',
    color: '#ff0000'
  };
  onMount(() => {
    const icon = new Icon({ target: document.body, props });
  });
</script>

1. Usages
<Icon name="add" />

2. Size
<Icon name="add" width="100" height="100" />
<Icon name="add" class="shrink-0 h-20 w-20" />

3. CSS HEX Colors
<Icon name="add" color="#c61515" />


4. CSS framworks suport

<Icon name="add" class="text-red-700 inline m-1" />


5. Dark mode

<Icon name="add" class="text-red-700 dark:text-green-500" />


6. aria-label

<Icon name="add" ariaLabel="red add" color="#c61515"/>

7. Unfocusable icon

<Icon name="add" tabindex="-1" />


8. Events

All icons have the following events:

- on:click
- on:keydown
- on:keyup
- on:focus
- on:blur
- on:mouseenter
- on:mouseleave
- on:mouseover
- on:mouseout

9. Passing down other attributes

<Icon name="add" tabindex="0" />


10 Using svelte:component

<svelte:component this="{Icon}" name="add"/>


11. Using onMount


12 Import all

{#each Object.keys(icons) as name}
<div class="flex gap-4 items-center text-lg">
  <Icon name={name} bind:width={size} bind:height={size} class="shrink-0"/>
  {name}
</div>
{/each}
