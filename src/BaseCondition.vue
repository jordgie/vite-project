<template>
    <div>
        <label for="name">Enter your name:</label>
        <input type="text" id="name" v-model="userName" />

        <div v-if="userName">
            <p>Hello, {{ userName }}!</p>
        </div>

        <div v-else>
            <p>Please enter your name.</p>
        </div>
    </div>
</template>

<script>
    export default {
        data() {
            return {
                userName: ""
            };
        }
    }
</script>