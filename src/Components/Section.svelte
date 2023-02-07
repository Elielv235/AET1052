<script lang="ts">
	import IntersectionObserver from "./IntersectionObserver.svelte";

  export let id: string;
</script>

<section {id}>
  <IntersectionObserver steps={100} threshold={50} let:visibleOnce>
    {#if visibleOnce}
      <slot />
    {/if}
  </IntersectionObserver>
</section>

<style lang="scss">
  section {
    min-height: 100vh;

    padding-top: 3.5rem;
  }
</style>

