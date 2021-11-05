<template>
        <div class="block">
            <p><span class="name">ID: </span><span>{{ list['id'] }}</span></p>
            <p><span class="name">Имя: </span><span>{{ list['first_name'] }}</span></p>
            <p><span class="name">Фамилия: </span><span>{{ list['last_name'] }}</span></p>
            <p><span class="name">Email: </span><span>{{ list['email'] }}</span></p>
            <p><span class="name">Пол: </span><span>{{ list['gender'] }}</span></p>
            <p><span class="name">ID адрес: </span><span>{{ list['ip_address'] }}</span></p>
        </div>
</template>

<script>
export default {
    props: ["list"],
    data() {
        return {
        }
    },
}
</script>

<style>
    .block {
        width: 350px;
        border: 3px solid black;
        margin: 10px;
        padding: 0 10px;
    }

    .name {
        font-weight: 700;
    }
</style>