<script context="module">
    let total = 1

    export const getTotal = () => {
        return total
    }
</script>
<script>
    let items = 1

    function addToCart() {
        items +=2
        total+=2
    }

</script>


<button on:click={addToCart}>Add me to Cart {items}</button>