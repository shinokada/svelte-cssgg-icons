<script>
  import { setContext } from 'svelte';
  import { Add } from '$lib';
  const iconCtx = {
    width: '200'
  };
  setContext('iconCtx', iconCtx);
</script>

<Add />
