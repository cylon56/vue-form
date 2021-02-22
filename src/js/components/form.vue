<template>
    <div>
        <input v-model="message" placeholder='Full Name'>
        <p>Name is: {{ capitalizeName }}</p>
    </div>
</template>

<script>
export default {
    name: `Form`,
    data() {
        return {
            message: ``
        }
    },
    computed: {
        capitalizeName() {
            return this.message.split(` `).map(s => s.charAt(0).toUpperCase() + s.slice(1)).join(` `)
        }
    },
}
</script>