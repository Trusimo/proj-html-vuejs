<template>
    <div class="container py-5">
        <div class="row">
            <div class="col-4">
                <h3>Grow Your Online Business Strategically, and Improve Customer Retention</h3>
                <div class="flex-social">
                    <i class="fa-brands fa-facebook-f"></i>
                    <i class="fa-brands fa-twitter"></i>
                    <i class="fa-brands fa-instagram"></i>
                    <i class="fa-brands fa-youtube"></i>
                    <i class="fa-brands fa-linkedin-in"></i>
                    <i class="fa-brands fa-tiktok"></i>
                </div>
            </div>
            <div class="col-2">
                <ul v-for="(item, index) in services" :key="index">
                    {{ item }}
                </ul>
            </div>
            <div class="col-2">
                <ul v-for="(item, index) in resources" :key="index">
                    {{ item }}
                </ul>
            </div>
            <div class="col-2">
                <ul v-for="(item, index) in company" :key="index">
                    {{ item }}
                </ul>
            </div>
            <div class="col-2">

            </div>
        </div>
        <div class="row mt-5 font-small">
            <div class="col-4">
                <i class="fa-solid fa-copyright"></i> 2020 Avada Consultant Powered by Wordpress
            </div>
            <div class="col-2">
                Call Us (555) 802-1234
            </div>
            <div class="col-2">

            </div>
            <div class="col-2">
                info@yourcompany.com
            </div>
        </div>

        <div class="live-chat shadow font-small">
            <div class="flex-img-foot">
                <img class="img-chat" src="../../public/marketing-expert-cta.png">
            </div>
            <div class="flex-x">X</div>
            This is a free HubSpot live chat. You can create your own chat flows
            and engage your customers with Avada & HubSpot!
        </div>
    </div>

</template>


<script>
export default {
    name: 'TheFooter',
    data() {
        return {
            services: [
                "Marketing plan",
                "Sales Development",
                "Digital Marketing",
                "Pricing",
                "Why Us",
                "Case Studies"
            ],
            resources: [
                "Learning Center",
                "Video Tutorial",
                "Customers",
                "Blog"
            ],
            company: [
                "Who We Are",
                "Contact Us",
                "Careers"
            ]

        }
    },
    methods: {

    }
}





</script>







<style>
.flex-social {
    display: flex;
    justify-content: flex-start;
    gap: 20px;
}

.live-chat {
    width: 180px;
    background-color: white;
    position: fixed;
    bottom: 15px;
    right: 10px;
    border-radius: 5px;
    padding: 5px 10px;
    z-index: 1;
}

.flex-x {
    display: flex;
    justify-content: end;
}

.flex-img-foot {
    display: flex;
    justify-content: center;
    position: relative;
}

.img-chat {
    width: 50px;
    height: 50px;
    border-radius: 50%;
    position: absolute;
    top: -40px
}
</style>