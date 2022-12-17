<script lang="ts">
    let number: number = 0

    $: positive = number > 0
    $: negative = number < 0

    export let ime: string
</script>

<div class="brojac">
    <button on:click={() => number--}>-</button>
    <p class:positive class:negative>{number}</p>
    <button on:click={() => number++}>+</button>
</div>
<div class="gumbici">
    <a class="natrag" href="./">Idi unatrag</a>
    <button class="btn" on:click={() => ime = ""}>Resetiraj ime</button>
</div>