<script>
  let count = 10;
</script>

<style>
  h1 {
    display: flex;
    margin-bottom: 4rem;
    font-size: 8rem;
    font-weight: 700;
  }

  span:first-of-type {
    margin-left: -3.5rem;
  }

  span:last-of-type {
    width: 50px;
    display: inline-block;
  }

  button {
    display: inline-block;
    padding: 1.5rem 5rem;
    color: inherit;
    font-family: inherit;
    font-size: 2rem;
    background: rgba(255, 255, 255, 0.05);
    border: 1px solid;
    border-radius: 10rem;
    transition: all 0.2s;
  }

  button:hover {
    background: rgba(255, 255, 255, 0.15);
    box-shadow: 0 0.3rem 0.5rem rgba(255, 255, 255, 0.15);
  }

  button:not(:last-child) {
    margin-right: 0.5rem;
  }
</style>

<h1>
  <span>Count:</span>
  &nbsp;
  <span>{count}</span>
</h1>

<div>
  <button on:click={() => (count += 1)}>+1</button>
  <button on:click={() => (count -= 1)}>-1</button>
  <button on:click={() => (count = 0)}>Reset</button>
</div>
