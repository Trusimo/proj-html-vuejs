<template>
    <div class="container">
        <div class="flex">
        <img src="../../public/avada-marketing-logo-2x-200x37.png" alt="">

        <!-- ciclo per le voci della navbar -->
        <div v-for="(voice, index) in navbarVoices" :key="index">
            {{ voice }}
        </div>

        <div>(555) 802-134</div>
        <button class="btn-orange">Free Quote</button>
    </div>
    </div>

</template>


<script>
export default {
    name: 'TheHeader',
    data() {
        return {
            navbarVoices: [
                "Home",
                "Services",
                "Why Us",
                "Case Studies",
                "About",
                "Blog"
            ]
        
}},
    methods: {

    }
}


</script>



<style>
header {
    position: fixed;
}
.flex {
    display: flex;
    justify-content: space-between;
    padding: 20px;
    align-items: center;
}

.btn-orange {
    border-style: none;
    background-color: #ffe7da;
    color: #f76210;
    padding: 5px 20px;
    border-radius: 8px;
}

.btn-orange:hover {
    background-color: #f76210;
    color: white;
}



</style>