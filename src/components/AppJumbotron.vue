<script>
export default {
    name: 'AppJumbotron',
    setup() {


        return {}
    }
}
</script>

<template>
    <div class="jumbotron d-flex align-items-end">
        <div class="text">
            <h2>current series</h2>
        </div>
    </div>
</template>


<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;

.jumbotron {
    height: 400px;
    background-image: url(../assets/img/jumbotron.jpg);
    background-position: top;
    background-size: cover;
    color: $dc_white;

    .text {
        padding: 0 0.5rem;
        margin-bottom: -20px;
        margin-left: 300px;
        background-color: $dc_primary;
    }
}
</style>