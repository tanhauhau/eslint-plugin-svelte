<div>
  {#each [] as e}
    A
    <!-- svelte-ignore a11y-label-has-associated-control a11y-no-noninteractive-tabindex -->
  {:else}
    <label tabindex="0">Click</label>
    <ul tabindex="0" />
  {/each}
</div>
