<script lang="ts">
    let inputC = $state(0);
    let inputF = $state(32);

    function calcConv(i: number, t: string){
        return Math.round((t=="F" ? (i * (9/5) + 32) : ((i - 32) * (5/9))) * 10) / 10
    }
</script>

C <input type="number" onkeyup={() => (inputF = calcConv(inputC, "F"))} bind:value={inputC}> - F <input type="number" onkeyup={() => (inputC = calcConv(inputF, "C"))} bind:value={inputF}>



<style>

</style>