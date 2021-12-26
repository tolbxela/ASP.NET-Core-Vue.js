<!-- Vue Component: Card -->

<template>
    <div v-bind:id="id" v-bind:name="name">
        <div class="card">
            <img v-bind:src="img" class="card-img-top p-2 bg-light border-bottom">
            <div class="card-body">
                <p class="card-text">
                    <slot></slot>
                </p>
            </div>
        </div>
    </div>
</template>

<script type="text/javascript">
    module.exports = {
        props: {
            id: String,
            name: String,
            img: String
        }
    }
</script>

<style scoped>
    .card {
        width: 15rem;
    }
</style>

<!-- End Vue Component -->