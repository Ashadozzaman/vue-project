<template>
<h1>Ashadozzaman Component</h1>
<h2>Id: {{Id}}</h2>
<h2>FullName: {{FullName}}</h2>
<h2>Degree: {{getStudentDetails('PSD').degree}}</h2>
<p>Data: {{getAllData()}}</p>
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
            }
        }
    },
    methods: {
        getAllData() {
            return {
                name: this.FullName,
                id: this.Id,
            }
        }
    }
}
</script>
