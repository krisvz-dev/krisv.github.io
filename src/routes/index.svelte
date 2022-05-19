<script>
  let money = 0;

  function increment() {
    money += 1;
  }
</script>
<button on:click={increment}>
  Pressed {money} times
</button>