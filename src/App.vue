<template>
    <div id="app">

        <my-app></my-app>

    </div>
</template>

<script>
    import Vue from 'vue';
    import wrap from '@vue/web-component-wrapper'
    import MyApp from './MyApp?shadow';

    const CustomElement = wrap(Vue, MyApp);
    window.customElements.define('my-app', CustomElement);

    export default {
        name: 'app'
    }
</script>
