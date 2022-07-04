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

        <!-- Case studies -->
        <div class="padding-sec">
            <h2 class="text-center">Trusted by Leading Organizations</h2>
            <div class="flex-partner row">
                <div class="col" v-for="(item, index) in caseStudies" :key="index">
                    <img :src="item.img" alt="">
                    <div class="bold">{{ item.par }}</div>
                    <h3>{{ item.number }}</h3>
                    <div class="font-small">{{ item.result }}</div>
                </div>
            </div>
            <button type="submit" class="btn-orange-col text-center">Read More Case Studies</button>
        </div>

        <!-- How we Boost -->
        <div class="padding-sec-lat">
            <div class="row my-5">
                <div class="col">
                    <h2>We Boost Our Clients Bottom Line by Optimizing Their Growth Potential</h2>
                    <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Doloribus dolorem, ducimus illo nostrum odit delectus</p>
                    <button type="submit" class="btn-orange-col">Why Work With Us</button>
                </div>
                <div class="col">
                    <img src="../../public/we-boost-our-clients-400x366.jpg" alt="">
                </div>
            </div>
        </div>

        <div class="padding-sec-lat">
            <div class="row">
                <div class="col">
                    <div class="padding-col">
                        <h4>We Build Relationships</h4>
                        <p class="font-small">Lorem ipsum dolor sit amet consectetur adipisicing elit. Consequuntur, libero id totam iusto esse impedit modi</p>
                    </div>
                    <div class="padding-col">
                        <h4>Proprietary Processes</h4>
                        <p class="font-small">Lorem ipsum dolor sit amet consectetur adipisicing elit. Consequuntur, libero id totam iusto esse impedit modi</p>
                    </div>
                </div>
                
                <div class="col padding-col">
                    <div>
                        <div><!-- iconafontawesome --></div>
                        <div v-for="(item, index) in qualities" :key="index">
                            <h5 class="padding-title">{{ item.title }}</h5>
                            <span class="font-small">{{ item.lorem }}</span>
                        </div>
                    </div>
                </div>
            </div>
        </div>

        <!-- Awards -->
        <div class="padding-sec">
            <h4 class="text-center">Awards</h4>
            <div class="row flex-partner">
            <div class="col" v-for="(prize, index) in awards" :key="index">
                <div><img :src="prize.img"></div>
                <span class="bold">{{prize.prizeName}}</span>
            </div>
        </div>
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
            ],
            caseStudies: [
                {
                    img: "../../public/case-studies-1.jpg",
                    par: "How Spaces attracted five millions visitors by improving the content",
                    number: "200%",
                    result: "Higher revenue from digital"
                },
                {
                    img: "../../public/case-studies-4.jpg",
                    par: "Creativity helped Hemisferio to increase their brand reach vertically",
                    number: "10x",
                    result: "Sales increase with the same AD spend"
                },
                {
                    img: "../../public/case-studies-6.jpg",
                    par: "How DigitalBox used AI-powered data insights to boost sales",
                    number: "3-year",
                    result: "Partnership with Avada Consultant"
                },
            ],
            qualities: [
                {
                    title: "Accountability",
                    lorem: "lorem ipsum lorem ipsum lorem"
                },
                {
                    title: "Transparency",
                    lorem: "lorem ipsum lorem ipsum lorem"
                },
                {
                    title: "Investment",
                    lorem: "lorem ipsum lorem ipsum lorem"
                }
            ],
            awards: [
                {
                img: "../../public/award-a-200x191.png",
                prizeName: "Winner Seo Master MAGT Smart Start Award 2017"
            },
                {
                img: "../../public/award-b-200x191.png",
                prizeName: "Top Social Media Agencies Next Partner 2018"
            },
                {
                img: "../../public/award-c-200x191.png",
                prizeName: "10 Fastest Growing Abstract Solution Providers 2019"
            },
                {
                img: "../../public/award-d-200x191.png",
                prizeName: "National Excellence Agencie Award Winner 2020"
            },
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

.padding-sec-lat {
    padding: 100px 50px;
}

.padding-title {
    padding-top: 20px;
}

.btn-orange-col {
    background-color: #f76210;
    color: white;
    border-style: none;
    border-radius: 8px;
    padding: 8px 30px;
}

.bold {
    font-weight: bold;
    font-size: 18px;
}

.font-small {
    font-size: 12px;
}

.padding-col {
    padding: 10px 30px;
}

</style>