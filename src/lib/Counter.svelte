<script>
    let count = $state(0);
    let doubled = $derived(count * 2);

    function onclick(){
        count++;
    }
</script>

<div>
    Clicked {count} times! That is {doubled} when doubled.
</div>
<button {onclick}>Click!</button>

<style>


</style>