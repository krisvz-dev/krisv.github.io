<script>
  let money = 0;
  let mpc = 1;
  let mpcCost = 25

  function increment() {
    money += mpc;
  }
  function buyMPC() {
    if (money >= mpcCost) {
      money -= mpcCost;
      mpc++;
    }
  }
</script>
<button on:click={increment}> Click! </button>
<h3>Money: {money}</h3>
<button on:click={buyMPC}>Buy +1 Money Per Click ${mpcCost}</button>
<h3>MPC: {mpc}</h3>