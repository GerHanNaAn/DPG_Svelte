<script>
  let vivsible = true;
  let red = true;
  let green = true;
  let blue = true;
  function action() {
    red = !red;
    blue = !blue;
    green = !green;
  }
</script>

<style>
  .square {
    width: 50px;
    height: 50px;
    margin: 10px;
    opacity: 1;
  }
  .squar__red {
    background: rgb(168, 13, 13);
  }
  .squar__blue {
    background: rgb(41, 76, 192);
  }
  .squar__green {
    background: rgb(103, 153, 28);
  }
  .row {
    display: flex;
    flex-direction: column;
    justify-content: center;
  }
  .hiden {
    opacity: 0;
  }
</style>

<div class="wrap">
  <div class="row">
    {#if red}
      <div on:click={action} class="square squar__red" />
    {/if}

    {#if !red}
      <div on:click={action} class="square squar__red hiden" />
    {/if}

    {#if blue}
      <div on:click={action} class="square squar__blue" />
    {/if}

    {#if !blue}
      <div on:click={action} class="square squar__blue hiden" />
    {/if}

    {#if green}
      <div on:click={action} class="square squar__green" />
    {/if}

    {#if !green}
      <div on:click={action} class="square squar__green hiden" />
    {/if}
  </div>
</div>
