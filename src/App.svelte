<script>
  let click = 0;
  let handle = (event) => {
    console.log(event);
    click += 1;
  };
</script>

<main>
  <button on:click={handle}>this button is is clicked {click} times</button>
</main>

<style>
</style>
