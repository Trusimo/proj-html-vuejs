<template>
    <div class="container padding-sec">
        <!-- 3 row centrali -->
        <div class="row">
            <div class="col">
                <img src="" alt="">
            </div>
            <div class="col">
                <h2>Increased Brand Awareness</h2>
                <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Doloribus dolorem, ducimus illo nostrum odit delectus</p>
                <button type="submit" class="btn-orange-col">Get a Consultation</button>
            </div>
        </div>

        <div class="row my-5">
            <div class="col">
                <h2>In-House Sales Training</h2>
                <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Doloribus dolorem, ducimus illo nostrum odit delectus</p>
                <button type="submit" class="btn-orange-col">Get a Consultation</button>
            </div>
            <div class="col">
                <img src="" alt="">
            </div>
        </div>

        <div class="row my-5">
            <div class="col">
                <img src="" alt="">
            </div>
            <div class="col">
                <h2>Harness Your Social Proof</h2>
                <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Doloribus dolorem, ducimus illo nostrum odit delectus</p>
                <button type="submit" class="btn-orange-col">Get a Consultation</button>
            </div>
        </div>

        <!-- Partners -->
        <h2 class="text-center">Some Brands We Work With</h2>
        <p class="text-center">Quisquie aliquet, libero consequat libero consectetur</p>

        <div class="flex-partner">
            <div v-for="(partner, index) in partners" :key="index">
                <img :src="partner.url">
            </div>
        </div>

        <div class="flex-partner shadow">
            <div>
                <img class="img-rounded" src="../../public/marketing-expert-cta.png" alt="">
            </div>
            <h5>Drive Leads and Sales with Avada</h5>
            <button class="btn-orange">(555) 802-134</button>
        </div>

    </div>

</template>


<script>
export default {
    name: 'TheMain',
    data() {
        return {
            partners: [
                {url: require('../../public/abstract.png')},
                {url: require('../../public/cglobal.png')},
                {url: require('../../public/next.png')},
                {url: require('../../public/hemisferio.png')},
                {url: require('../../public/spaces.png')},
                {url: require('../../public/digitalbox.png')},
            ]
        
}},
    methods: {

    }
}







</script>







<style>

.flex-partner {
    display: flex;
    justify-content: space-between;
    padding: 30px 0;
    align-items: center;

}

.padding-sec {
    padding: 100px 0;
}

.btn-orange-col {
    background-color: #f76210;
    color: white;
    border-style: none;
    border-radius: 8px;
    padding: 8px 30px;
}

</style>