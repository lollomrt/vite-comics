<script>
import { stringifyExpression } from '@vue/compiler-core';

export default {
    props: {
        img: String,
        title: String
    }
}
</script>

<template lang="">
    <div class="card">
        <img src="img" alt="">
        <h3>{{ title }}</h3>
    </div>
</template>

<style lang="scss">

</style>