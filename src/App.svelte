<script>
  // const name = "Sam allen";
  // const ht = "<h2><em>Sam<em/>Allen<h2/>";
  // const alt = "This is an alt text";
  // const disabled = true;
  // const theme = "blk";
  // const size = "med";
  // const finished = true;
  let age = 17;
</script>

<main>
  <!-- <h2>Hello Mr.{name}</h2>
  <h1>This is from script :{@html ht}</h1>
  <img {alt} />
  <button {disabled}>this a button</button>
  <h2 class={(finished ? "finished" : "", theme)}>This is for class binding</h2>
  <h2 class={size}>This is for class binding</h2> -->
  {#if age >= 18}
    <h3>You are eligible to vote</h3>
  {:else if age === 17}
    <h3>Dont worry you can vote in a year</h3>
  {:else}
    <h3>You are not elgible to vote</h3>
  {/if}
</main>

<style>
  .lar {
    font-size: 3em;
  }
  .med {
    font-size: 3em;
  }
  .blk {
    background-color: #333;
    color: #fff;
  }
  .wht {
    background-color: #fff;
    color: #333;
  }
  .finished {
    text-decoration: line-through;
  }
  h1 {
    color: #f25fff;
  }
</style>
