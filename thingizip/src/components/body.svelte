<script>
  import Home from './home.svelte';
  import RecentsPage from './recentsPage.svelte';
  import Info from './info.svelte';
  import { valueStore } from '../utils/valueStore';
</script>

<div class="p-4 mb-6">
  {#if $valueStore == 'Home'}
    <Home />
  {:else if $valueStore == 'Recents'}
    <RecentsPage />
  {:else if $valueStore == 'Info'}
    <Info />
  {/if}
</div>
