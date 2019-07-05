<script>
  import "./Ponder.jpg";
  let count = 0;
  let counter = 0;
  function handleClick() {
    count += 1;
  }

  function onClick() {
    count -= 1;
  }

  function plusOne() {
    counter += 1;
  }

  function minusOne() {
    counter -= 1;
  }
</script>

<style>
  .player1 {
    position: fixed;
    top: 15%;
    left: 50%;
    /* bring your own prefixes */
    transform: translate(-50%, -50%);
    display: block;
    color: #fff;
  }

  .add {
    position: fixed;
    top: 75%;
    left: 50%;
    /* bring your own prefixes */
    transform: translate(-50%, -50%);
    display: block;
  }
  .minus {
    position: fixed;
    top: 80%;
    left: 50%;
    /* bring your own prefixes */
    transform: translate(-50%, -50%);
    display: block;
  }
  .score1 {
    position: fixed;
    top: 63%;
    left: 50%;
    /* bring your own prefixes */
    transform: translate(-50%, -50%);
    display: block;
    font-size: 30px;
    color: #fff;
  }

  .add1 {
    position: fixed;
    top: 35%;
    left: 50%;
    /* bring your own prefixes */
    transform: translate(-50%, -50%);
    display: block;
  }

  .minus1 {
    position: fixed;
    top: 40%;
    left: 50%;
    /* bring your own prefixes */
    transform: translate(-50%, -50%);
    display: block;
  }

  .score2 {
    position: fixed;
    top: 23%;
    left: 50%;
    /* bring your own prefixes */
    transform: translate(-50%, -50%);
    display: block;
    font-size: 30px;
    color: #fff;
  }

  .player2 {
    position: fixed;
    top: 55%;
    left: 50%;
    /* bring your own prefixes */
    transform: translate(-50%, -50%);
    display: block;
    color: #fff;
  }

  :global(body) {
    background: url("https://res.cloudinary.com/lmn/image/upload/e_sharpen:100/f_auto,fl_lossy,q_auto/v1/gameskinnyc/u/n/t/untitled-aabda.jpg")
      no-repeat fixed center;
    background-size: cover;
  }
</style>

<body>
<div class="maindiv">
<h2 class="player1">Player 1</h2>
<p class="score1">{count}</p>
<div class="add">
<button on:click={handleClick}>
+1
</button>
</div>


<div class="minus">
<button on:click={onClick}>
-1
</button>
</div>


<h2 class="player2">Player 2</h2>
<p class="score2">{counter}</p>
<div class="add1">
<button on:click={plusOne}>
+1
</button>
</div>


<div class="minus1">
<button on:click={minusOne}>
-1
</button>
</div>

</div>
</body>
