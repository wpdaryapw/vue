<template>
    <div class="header">
        <div class="main">
            <h2 v-for="elem in data" class="text">
                {{ elem.title }}
            </h2>
        </div>
        <div class="textes">
            <div class="text_f">
                <h1>Alex <br/> Wylliam</h1>
            </div>
            <div class="text_s"> 
                <h2>web developer
                <br/>28 years old, Karaganda</h2>
            </div>
            <div class="lang_main">
                <h3 class="lang_g">RU </h3>
                <h3 class="lang">| ENG</h3>
            </div>
        </div>
        <div class="photo">
            <img src="../assets/BSPP2266.jpg" class="pic"/>
        </div>
    </div>
</template>



<script>

export default {
    data() {
        return {
            data: [
                { id: 1, title: 'Home' },
                { id: 2, title: 'About me' },
                { id: 3, title: 'Skills' },
                { id: 4, title: 'Portfolio' },
                { id: 5, title: 'Contacts' },
            ]
        }
    }
}
</script>


<style scoped>

.header{
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
}

.main {
    display: flex;
    flex-direction: row;
    justify-content: center;
    color: #828282;
    font-family: Abel;
    font-size: 18px;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
    text-align: center;
    padding: 33px;
    position: relative;
}

.text {
    display: flex;
    flex-direction: row;
    justify-content: center;
    padding-left: 177px;
    border-bottom: 1px solid #828282;;
    color: #828282;
font-family: Abel;
font-size: 18px;
font-style: normal;
font-weight: 400;
line-height: normal;
}
.text:first-child {
    padding-left: 0;
}
.textfirst-child {
    margin-left: 0;
}

h3{
    transform-origin: top left;
    transform: rotate(270deg);
}
.lang_main{
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
}
.lang{
    color: #000;
    font-family: Abel;
    font-size: 16px;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
}

.lang_g{
    position: absolute;
    top: 310px;
    right: 485px;
    color: #828282;
    font-family: Abel;
    font-size: 16px;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
}

.textes{
    display: flex;
    flex-direction: row;
    text-align: center;
    justify-content: center;
    gap: 210px;
    text-align: center;
}
.text_f{
    color: var(--Black, #070707);
    font-family: Abel;
    font-size: 47.339px;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
}
.text_s{
    display: flex;
    flex-direction: column;
    justify-content: center;
    text-align: center;
    color: var(--Black, #070707);
    font-family: Abel;
    font-size: 18px;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
}

.photo{
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
}

</style>
