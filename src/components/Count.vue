<script>



export default {

    name: 'Count',

    emit: ['increment', 'decrement']

}

</script>


<template>
    <div class="col-12 text-center">
        <button @click="$emit('decrement')" class="btn btn-success me-3">-</button>
        <button @click="$emit('increment')" class="btn btn-danger">+</button>
    </div>
</template>


<style></style>