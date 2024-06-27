<script>
    let count = 0

    function increment() {
        count++
    }

    function decrement() {
        count--
    }
</script>

<div class="container">
<h1>A counting App</h1>

<div class="count_container">
    <button on:click={decrement}>-</button>
    <p>{count}</p>
    <button on:click={increment}>+</button>
</div>
</div>

<style>
    .container {
        display: flex;
        flex-flow: column nowrap;
        align-items: center;
        margin-top: 5rem;
    }

    h1 {
        font-size: 3rem;
        margin-bottom: 5rem;
        color: rgb(68, 68, 68);
    }

    .count_container {
        margin-bottom: 2rem;
        width: min(90% , 450px);
        height: auto;
        display: flex;
        flex-flow: row nowrap;
        align-items: center;
    }

    button {
        padding: 0.5rem 1.2rem;
        flex:1 0 30%;
        font-size: 2.5rem;
        font-weight: bold;
        border:1px solid black;
        border-radius: 8px;
        background: none;
    }

    button:active {
        transform:scale(1.02);
    }

    p {
        font-size: 2.5rem;
        flex:1 0 30%;
      
        padding: 1.2rem 1.2rem;
        text-align: center;
    }



    
</style>