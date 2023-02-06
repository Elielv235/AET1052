<script lang="ts">
	import IntersectionObserver from './../Components/IntersectionObserver.svelte';
	import Welcome from './../Components/Welcome.svelte';
  import "../Styling/global.scss"
</script>

<IntersectionObserver steps={100} threshold={50} let:visibleOnce>
  {#if visibleOnce}
    <Welcome />
  {/if}
</IntersectionObserver>
