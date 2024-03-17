<script>
    let name = "Svelte"
    let counter = 0;

    $: counterClass = counter % 2 === 0 ? 'red' : 'blue';

    $: upperName = name.toUpperCase();
    $: lowerName = name.toLowerCase();

    function chaneName() {
        name = "New name";
    }


</script>

<style>
    .blue {
        color: blue;
    }

    .red {
        color: red;
    }
</style>

<h1>{name}</h1>
<h2>{upperName}</h2>
<h2>{lowerName}</h2>

<button on:click={chaneName}>Change name</button>

<h1 class={counterClass}>Counter {counter}</h1>
<button on:click={() => counter++}>Add 1 to counter</button>