<script>
  export let title;
  export let grow;
  export let show_title = true;
</script>

<div style={`flex-grow: ${grow}`}>
  {#if show_title}
    <h1>{title}</h1>
  {/if}
  <slot />
</div>

<style>
  div {
    display: flex;
    flex-direction: column;
    justify-content: flex-start;
    align-items: center;
    /* background-color: rgba(46, 77, 72, 0.6); */
    margin-left: var(--global_margin);
  }
  div > h1 {
  }
</style>
