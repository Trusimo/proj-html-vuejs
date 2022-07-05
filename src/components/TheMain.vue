<template>

    <div>
        <div class="container padding-sec">
            <!-- 3 row centrali -->
            <div class="row">
                <div class="col p-5">
                    <img src="../../public/beer_thumbnail-400x300.jpg" alt="">
                </div>
                <div class="col p-5">
                    <h2>Increased Brand Awareness</h2>
                    <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Doloribus dolorem, ducimus illo nostrum
                        odit delectus Lorem ipsum, dolor sit amet consectetur adipisicing elit. Ipsa sed at officia omnis perferendi</p>
                    <button type="submit" class="btn-orange-col">Get a Consultation</button>
                </div>
            </div>

            <div class="row my-5">
                <div class="col p-5">
                    <h2>In-House Sales Training</h2>
                    <p>orem ipsum dolor, sit amet consectetur adipisicing elit. Doloribus dolorem, ducimus illo nostrum
                        odit delectus Lorem ipsum, dolor sit amet consectetur adipisicing elit. Ipsa sed at officia omnis perferendi</p>
                    <button type="submit" class="btn-orange-col">Get a Consultation</button>
                </div>
                <div class="col p-5">
                    <img src="../../public/cafe_thumbnail-400x300.jpg" alt="">
                </div>
            </div>

            <div class="row my-5">
                <div class="col p-5">
                    <img src="../../public/cleaning_services-400x300.jpg" alt="">
                </div>
                <div class="col p-5">
                    <h2>Harness Your Social Proof</h2>
                    <p>orem ipsum dolor, sit amet consectetur adipisicing elit. Doloribus dolorem, ducimus illo nostrum
                        odit delectus Lorem ipsum, dolor sit amet consectetur adipisicing elit. Ipsa sed at officia omnis perferendi</p>
                    <button type="submit" class="btn-orange-col">Get a Consultation</button>
                </div>
            </div>
        </div>

        <!-- Partners -->
        <div class="container">
            <h2 class="text-center">Some Brands We Work With</h2>
            <p class="text-center">Quisquie aliquet, libero consequat libero consectetur</p>

            <div class="flex-partner">
                <div v-for="(partner, index) in partners" :key="index">
                    <img :src="partner.url">
                </div>
            </div>
        </div>

        <div class="container flex-partner shadow">
            <div>
                <img class="img-rounded" src="../../public/marketing-expert-cta.png" alt="">
            </div>
            <h5>Drive Leads and Sales with Avada</h5>
            <button class="btn-orange">(555) 802-134</button>
        </div>

        <!-- Case studies -->
        <div class="container padding-sec">
            <h2 class="text-center">Trusted by Leading Organizations</h2>
            <div class="flex-case row">
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
        <div class="container padding-sec-lat">
            <div class="row">
                <div class="col">

                </div>
                <div class="col-5 px-5">
                    <h2>We Boost Our Clients Bottom Line by Optimizing Their Growth Potential</h2>
                    <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Doloribus dolorem, ducimus illo nostrum
                        odit delectus</p>
                    <button type="submit" class="btn-orange-col">Why Work With Us</button>
                </div>
                <div class="col-5 px-5">
                    <img src="../../public/we-boost-our-clients-400x366.jpg" alt="">
                </div>
                <div class="col">

                </div>
            </div>
        </div>

        <div class="container padding-sec-lat">
            <div class="row">
                <div class="col">

                </div>
                <div class="col-5 p-5">
                    <h4>We Build Relationships</h4>
                    <p class="font-small">Lorem ipsum dolor sit amet consectetur adipisicing elit. Consequuntur,
                        libero
                        id totam iusto esse impedit modi</p>
                    <h4>Proprietary Processes</h4>
                    <p class="font-small">Lorem ipsum dolor sit amet consectetur adipisicing elit. Consequuntur,
                        libero
                        id totam iusto esse impedit modi</p>
                </div>

                <div class="col-5">
                    <div>
                        <div>
                            <!-- iconafontawesome -->
                        </div>
                        <div v-for="(item, index) in qualities" :key="index">
                            <h5 class="padding-title">{{ item.title }}</h5>
                            <span class="font-small">{{ item.lorem }}</span>
                        </div>
                    </div>
                </div>
                <div class="col">

                </div>
            </div>
        </div>

        <!-- Awards -->
        <div class="container padding-sec">
            <h4 class="text-center">Awards</h4>
            <div class="row flex-partner">
                <div class="col text-center" v-for="(prize, index) in awards" :key="index">
                    <div><img :src="prize.img"></div>
                    <span class="bold">{{ prize.prizeName }}</span>
                </div>
            </div>
        </div>

        <!-- worker quote -->
        <div class="container padding-sec-lat">
            <div class="row">
                <div class="col">

                </div>
                <div class="col-6">
                    <img src="../../public/large-testimonial-400x389.jpg" alt="">
                </div>
                <div class="col-4 p-5">
                    <p class="bold text-left">"The team at Avada Marketing Consultant is faboulous. They helped us
                        unlock
                        our potential
                        online and offline. We have experienced year on year growth due to their progressive approach"
                    </p>
                    <p class="font-small bold">Kate Schneider</p>
                    <span class="font-small">Marketing Consultant - Abstract</span>
                </div>
                <div class="col">

                </div>
            </div>
        </div>

        <!-- Marketing resources -->
        <div class="container padding-sec">
            <div class="row">
                <div class="col">
                    <h2>Marketing Resources: Insider Advice on How to Increase Sales</h2>
                </div>
                <div class="col flex-bottom">
                    <button type="submit" class="btn-orange-col">Explore All Resources</button>
                </div>
            </div>

            <div class="flex-case row">
                <div class="col" v-for="(item, index) in marketingTips" :key="index">
                    <img :src="item.img" alt="">
                    <h4 class="py-3">{{ item.text }}</h4>
                </div>
            </div>
        </div>

        <!-- sfondo nero -->
        <div class="bg-black">
            <div class="container padding-sec">
                <div class="row">
                    <div class="col">
                        <h2>Let's Make Things Happen</h2>
                        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. A neque assumenda vitae earum?
                            Praesentium
                        </p>
                        <div class="line"></div>
                        <div class="font-small py-3">
                            "The team at Avada Marketing Consultant is faboulous. They helped us
                            unlock
                            our potential
                            online and offline. We have experienced year on year growth due to their progressive
                            approach"
                        </div>
                        <div class="font-small py-3">George Anderson</div>
                        <div class="font-small">DigitalBox CEO</div>

                    </div>
                    <div class="col-5">

                    </div>
                    <div class="col px-5">
                        <div class="form-black">
                            <div class="flex-form">
                                <img class="img-rounded" src="/marketing-consultant-expert.jpg" alt="">
                                <h5 class="color-bl">Richard Madsen</h5>
                                <p class="color-bl">Marketing Consulant Expert</p>
                            </div>
                            <form>
                                <div class="form-group">
                                    <input type="name" class="form-control" placeholder="Your name*">
                                </div>
                                <div class="form-group">
                                    <input type="email" class="form-control" placeholder="Your email*">
                                </div>
                                <div class="form-group">
                                    <input type="name" class="form-control" placeholder="Your phone number*">
                                </div>
                                <button type="submit" class="btn-orange-variant">Get a Callback</button>
                                <div class="condition-font">By submitting my data I agree to be contacted</div>
                            </form>
                        </div>
                    </div>
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
                { url: require('../../public/abstract.png') },
                { url: require('../../public/cglobal.png') },
                { url: require('../../public/next.png') },
                { url: require('../../public/hemisferio.png') },
                { url: require('../../public/spaces.png') },
                { url: require('../../public/digitalbox.png') },
            ],
            caseStudies: [
                {
                    img: "../../case-studies-1-400x450.jpg",
                    par: "How Spaces attracted five millions visitors by improving the content",
                    number: "200%",
                    result: "Higher revenue from digital"
                },
                {
                    img: "../../case-studies-4-400x450.jpg",
                    par: "Creativity helped Hemisferio to increase their brand reach vertically",
                    number: "10x",
                    result: "Sales increase with the same AD spend"
                },
                {
                    img: "../../case-studies-6-400x450.jpg",
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
                    img: "../../award-a-200x191.png",
                    prizeName: "Winner Seo Master MAGT Smart Start Award 2017"
                },
                {
                    img: "../../award-b-200x191.png",
                    prizeName: "Top Social Media Agencies Next Partner 2018"
                },
                {
                    img: "../../award-c-200x191.png",
                    prizeName: "10 Fastest Growing Abstract Solution Providers 2019"
                },
                {
                    img: "../../award-d-200x191.png",
                    prizeName: "National Excellence Agencie Award Winner 2020"
                },
            ],
            marketingTips: [
                {
                    img: "../../blog-posts-6-400x267.jpg",
                    text: "Marketing Tips and Tricks For Your Website"
                },
                {
                    img: "../../blog-posts-5-400x267.jpg",
                    text: "How to Write Stunning Blog Post Titles"
                },
                {
                    img: "../../blog-posts-4-400x267.jpg",
                    text: "Techniques to Reduce Facebook ADS Spends"
                }
            ]

        }
    },
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

.flex-case {
    display: flex;
    justify-content: space-between;
    padding: 30px 0;
    align-items: center;
    gap: 10px
}

.flex-bottom {
    display: flex;
    justify-content: end;
    align-items: flex-end;
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


.bg-black {
    background-color: black;
    color: white;
    width: 100%;
}

.line {
    width: 46px;
    border: 1px solid rgb(79, 78, 78)
}

.form-black {
    background-color: white;
    padding: 20px;
    border-radius: 8px;
}
</style>