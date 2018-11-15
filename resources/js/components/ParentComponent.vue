<template>
    <div class="container">
        <div class="row justify-content-center">
            <example-component v-model="searchText"></example-component>
            <example-component v-model="searchText2"></example-component>
        </div>
    </div>
</template>

<script>
    export default {
        mounted() {
            console.log('Component parent mounted.');
        },
        data() {
            return {
                searchText: '',
                searchText2: '',
            }
        }
    }
</script>
