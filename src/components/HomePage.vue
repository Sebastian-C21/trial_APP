<template>
    <div class="homepage">
        <h1>Trying to add a new component </h1>
        <h2> {{ messagee }}</h2>
        <b-list-group>
            <b-list-group-item v-for="item in itmes">
                {{ item.message }}
            </b-list-group-item>
        </b-list-group>
        <b-list-group>
            <b-list-group-item v-for="item in jum">
                {{ item }}
            </b-list-group-item>
        </b-list-group>
        <div>
            <button> clickear para no sé </button>
            <div>{{ cont }}</div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'homepage',
    data () {
        return {
            messagee: 'Destination breakdown',
            itmes: [
            { message: 'Spaghetti'},
            { message: 'Tomato'},
            { message: 'Cheese'},
            { message: 'nose'},
            { message: 'Camilo'},
            { message:'Nickolas'}, ],
            jum: ['xd','yolo','swag'],
            cont: 1
        }
    },
    methods: {
        contador: function() {
            cont += 1
        }
    }
}
</script>

<style scoped>
h1, h2 {
    background-color: blueviolet;
}
</style>