<script>
  let foo

  const remove1 = () => {
    foo?.remove()
  }
  const remove2 = () => {
    // eslint-disable-next-line no-unsafe-optional-chaining -- ignore
    ;(foo?.remove)()
  }
</script>

<p bind:this={foo}>div</p>

<button on:click={() => remove1()}>Click Me</button>
<button on:click={() => remove2()}>Click Me</button>
