<template>
    <div id="test">
        <div class="well">
            Well no shadow dom

            <select name="" id="" class="form-control">
                <option value="">Teste</option>
                <option value="">Teste</option>
                <option value="">Teste</option>
            </select>
        </div>
    </div>
</template>

<script>
    export default {
        name: "MyApp",
        beforeCreate() {
            this.axios.get('/test');
        }
    }
</script>

<style>
    @import '../node_modules/bootstrap/dist/css/bootstrap.min.css';
    @import '../node_modules/bootstrap-vue/dist/bootstrap-vue.min.css';

    p {
        color: red
    }
</style>
