<template>
    <div class="about_me">
        <div class="about_main">
            <h1 class="main_t">
                About me
            </h1>
            <div class="text">
                <p>
                    Hi, I'm Alex – web developer from Karaganda. 
                    <br/>I'm interested in development and everything connected with it.
                </p>
                <p>
                    Ready to implement excellent projects
                    <br/>with wonderful people.
                </p>
            </div>
        </div>
    </div>
</template>

<script>
</script>

<style scoped>
    * {
        background-color: #F6F6F6;
    }
    .main_t {
        color: var(--Black, #070707);
        text-align: center;
        font-family: Abel;
        font-size: 34px;
        font-style: normal;
        font-weight: 400;
        line-height: normal;
    }
    .text {
        color: var(--Black, #070707);
        text-align: center;
        font-family: Abel;
        font-size: 18px;
        font-style: normal;
        font-weight: 400;
        line-height: normal;
        margin-top: 20px; /* Добавляем отступ сверху */
        margin-bottom: 20px; /* Добавляем отступ снизу */
    }

    p{
        margin-bottom: 70px;
    }
    .about_main {
        padding-top: 100px;
        padding-bottom: 150px;
    }
</style>
