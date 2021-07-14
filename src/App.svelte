<script>
  // const name = "Sam allen";
  // const ht = "<h2><em>Sam<em/>Allen<h2/>";
  // const alt = "This is an alt text";
  // const disabled = true;
  // const theme = "blk";
  // const size = "med";
  // const finished = true;
  const myfav = ["Asta", "Yuno", "Noelle"];
  const hate = [];
</script>

<main>
  <!-- <h2>Hello Mr.{name}</h2>
  <h1>This is from script :{@html ht}</h1>
  <img {alt} />
  <button {disabled}>this a button</button>
  <h2 class={(finished ? "finished" : "", theme)}>This is for class binding</h2>
  <h2 class={size}>This is for class binding</h2> -->
  <h3>My fav characters in Black Clover</h3>
  {#each myfav as item, no}
    <strong>{no + 1}.{item}</strong>
    <br />
  {/each}
  {#each hate as it}
    {it}
  {:else}
    <h3>I dont hate any characters</h3>
  {/each}
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
