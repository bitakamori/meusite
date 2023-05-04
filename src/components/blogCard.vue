<script>
import { stringifyQuery } from 'vue-router';


export default {
    props: {
        nome: String,
        data: String,
        path: String
    }
}
</script>


<template>
    <div class="card">
        <div class="imgCard">
            <img :src="path" alt="">
        </div>
        <div class="textCard">
            <div style="font-weight: 400; margin-bottom: 5px;">
                {{ nome }}
            </div>
            <div>
                {{ data }}
            </div>
        </div>
    </div>
</template>

<style scoped>
.card {
    display: flex;
    flex-direction: row;
    justify-content: space-between;

    height: 150px;
    width: 400px;

    margin: 5px;

    box-shadow: 3px 3px 3px rgb(7, 7, 7);
    border-radius: 20px;
    background-color: #212121;
    transition: 0.6s ease-in-out;
}

.card:hover {
    box-shadow: 0px 0px 3px rgb(36, 36, 36);
}

img {
    width: auto;
    height: 125px;
    border-radius: 10px;

    box-shadow: 2px 2px 5px black;

}

.imgCard {
    width: 250px;

    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
}

.textCard {
    width: 100%;

    display: flex;
    flex-direction: column;
    justify-content: center;

    align-items: right;
    padding: 10px;

    font-weight: 200;


    border-left: 1px solid rgb(48, 48, 48);
}
</style>
