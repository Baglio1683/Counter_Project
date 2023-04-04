<script>
import { propsToAttrMap } from '@vue/shared';


export default{
    name: "Counter", 

   props: {

    counter: Number

   }

}

</script>

<template>

<p class="col-12 text-center">{{ this.counter }}</p>

</template>

<script scoped>

</script>