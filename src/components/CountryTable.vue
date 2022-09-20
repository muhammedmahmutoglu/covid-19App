<template>
    <table class="table">
        <thead>
            <tr>
                <th scope="col">#</th>
                <th scope="col">Date</th>
                <th scope="col">Confirmed</th>
                <th scope="col">Deaths</th>
                <th scope="col">Recovered</th>
            </tr>
        </thead>
        <tbody>
            <tr v-for="(item, index) in data" :key="index">
                <th scope="row">{{index + 1}}</th>
                <td>{{item.Date}}</td>
                <td>{{item.Confirmed }}</td>
                <td>{{item.Deaths}}</td>
                <td>{{item.Recovered }}</td>
            </tr>
        </tbody>
    </table>
</template>

<script>
export default {
    props: ['data']
}
</script>