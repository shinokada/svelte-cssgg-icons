<script>
  import { setContext } from 'svelte';
  import { Add, Youtube } from '$lib';
  const iconCtx = {
    size: '200',
    color: '#0000ff'
  };
  setContext('iconCtx', iconCtx);
</script>

<Add />
<Youtube />
