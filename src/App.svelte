<script>
  const name = "Sam allen";
  const ht = "<h2><em>Sam<em/>Allen<h2/>";
  const alt = "This is an alt text";
  const disabled = true;
</script>

<main>
  <h2>Hello Mr.{name}</h2>
  <h1>This is from script :{@html ht}</h1>
  <img {alt} />
  <button {disabled}>this a button</button>
</main>

<style>
  h1 {
    color: #f25fff;
  }
</style>
