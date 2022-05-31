<template>
<h1> Component</h1>
<!-- <h2>Id: {{Id}}</h2>
<h2>FullName: {{FullName}}</h2> 
<h2>Degree: {{getStudentDetails('PSD').degree}}</h2>
<p>Data: {{getAllData()}}</p> -->
<button v-on:click="clickEvent()">Button 1</button>
<button v-on:dblclick="dblclickEvent()">Button DBL</button><br>
<input type="text" v-model="count">
<!-- v-modela use for two data binding -->

<h2>{{count}}</h2>
</template>

<script>
export default {
    name: "AshadozzamanShvou",
    data() {
        return {
            Id: 1,
            FullName: 'Ashadozzaman Shvou',
            getStudentDetails: function (a) {
                return {
                    degree: a,
                    vercity: 'GU',
                };
            },
            count: 0,
        }
    },
    methods: {
        getAllData() {
            return {
                name: this.FullName,
                id: this.Id,
            }
        },
        clickEvent() {
            this.count = this.count + 1;
        },
        dblclickEvent() {
            alert('dbl click');
        }
    }
}
</script>
