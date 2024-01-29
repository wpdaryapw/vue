<template>
    <div class="main">
        <div class="text_f">
            <h1>Contacts</h1>
        </div>
        <div class="text_s">
            <h2>Want to know more or just chat? <br/>You are welcome!</h2>
        </div>
        <div class="button-container">
            <div class="pic">
                <img src="../assets/Group 2.png"/>
                <img src="../assets/Group 8.png"/>
                <img src="../assets/Group 9.png"/>
                <img src="../assets/Group 10.png"/>
            </div>
            <button class="oval-button">Send message</button>
        </div>
        <div class="text_t">
            <h2>Like me on <br/>LinkedIn, Instagram, Behance, Dribble</h2>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            data: []
        }
    }
}
</script>

<style scoped>
* {
    background-color: #F6F6F6;
}

.main{
    display: flex;
    flex-direction: column;
    align-items: center;
    padding-top: 100px;
    padding-bottom: 150px;
}

.text_f {
    color: var(--Black, #070707);
    text-align: center;
    font-family: Abel;
    font-size: 34px;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
    padding-bottom: 20px;
}

.text_s{
    color: var(--Black, #070707);
    text-align: center;
    font-family: Abel;
    font-size: 18px;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
}

.text_t{
    color: #828282;
    text-align: center;
    font-family: Abel;
    font-size: 14px;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
}

.button-container {
    margin-top: 20px; /* Расстояние между текстом и кнопкой */
}

.oval-button {
    width: 166.461px;
    height: 38px;
    flex-shrink: 0;
    color: #FFF;
    text-align: center;
    font-family: Abel;
    font-size: 18px;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
    background-color: #000;
    border: none;
    border-radius: 19px; /* половина высоты для овальной формы */
}

.pic{
    gap: 50px;
}
</style>
