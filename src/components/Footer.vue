<template>
    <footer class="footer">
        <div class="container">
            <span v-html="settings.footer" />
        </div>
    </footer>
</template>

<script>import Vue from 'vue';
import App from './App';
import VueSplide from '@splidejs/vue-splide';

Vue.use( VueSplide );

new Vue( {
  el    : '#app',
  render: h => h( App ),
} );
export default {
    data() {
        return {
            settings: require("../../data/theme.json")
        }
    }
}
</script>

<style scoped>
.footer {
    font-size: 0.8rem;
    padding: 6rem 0;
}
</style>
