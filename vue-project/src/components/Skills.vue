<template>
    <div class="skills">
        <div class="skills-text">
            <h2>Skills</h2>
        </div>
        <div class="skills-text-second">
            <p>I work in such technologies as</p>
        </div>
        <div class="card-main">
            <div class="card" v-for="elem in data" :key="elem.id">
                <img :src="elem.image" class="img"/>
                <p>{{ elem.title }}</p>
                <div class="rating">
                    <span v-for="i in 5" :key="i" :class="[ 'fa', 'fa-star', { 'active': i <= elem.rate, 'inactive': i > elem.rate } ]"></span>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            data: [
                { id: 1, title: 'HTML5', rate: 4, image: '../image 1.png' },
                { id: 2, title: 'CSS3', rate: 3, image: '../image 2.png' },
                { id: 3, title: 'JavaScript', rate: 4, image: '../image 3.png' },
                { id: 4, title: 'React', rate: 5, image: '../image 6.png' },
            ],
        };
    },
}
</script>

<style scoped>
.skills {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    margin-bottom: 100px;
}
.img{
    width: 88px;
    height: 88px;
    padding-bottom: 25px;
}
.skills-text {
    color: var(--Black, #070707);
    text-align: center;
    font-family: 'Abel';
    font-size: 34px;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
    padding-bottom: 69px;
}

.skills-text-second {
    color: var(--Black, #070707);
    text-align: center;
    font-family: 'Abel';
    font-size: 18px;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
}

.card-main {
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: space-evenly;
    gap: 90px;
    padding: 60px;
}

.card {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: space-evenly;
    width: 100%;
}

.card > p {
    color: #828282;
    font-family: 'Abel';
    font-size: 14px;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
}

.rating {
    display: flex;
    flex-direction: row;
    color: #828282;
    font-size: 18px;
    padding-top: 40px;
}

.rating .fa {
    margin-right: 5px;
}

.rating .fa.active {
    color: orange;
}

.rating .fa.inactive {
    color: #E5E5E5; 
}
</style>
