<script lang="ts">
    import Brojac from "$lib/components/brojac.svelte"
    import Unos from "$lib/components/unos.svelte"

    export let ime: string
</script>
<Unos bind:ime/>
<Brojac bind:ime/>