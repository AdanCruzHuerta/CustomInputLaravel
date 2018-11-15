<template>
    <div class="container">
        <div class="row justify-content-center">
            <div class="col-md-8">
                <div class="card card-default">
                    <div class="card-header">Example Component</div>

                    <div class="card-body">
                        <input type="text" class="form-control" v-bind:value="value" v-on:input="$emit('input', $event.target.value)">
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        props: ['value'],
        mounted() {
            console.log('Component mounted.');
            this.ready();
        },
        methods: {
            ready(){
                console.log('ready');
            }
        }
    }
</script>
