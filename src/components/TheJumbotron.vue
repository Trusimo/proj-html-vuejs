<template>
    <div class="bg-jumbo">
        <div class="container">
            <section>
                <div class="row">
                <div class="col padding-col">
                    <h1>Unlock Your Online Growth Potential</h1>
                    <p>Online marketing to secure customer retention, leads and sales.
                        We focus on the bigger picture.
                    </p>
                    <button class="btn-white">Our Services</button>
                </div>
                <div class="col">

                </div>
            </div>
                <div class="form-absolute">
                    <div class="flex-form">
                        <img class="img-rounded" src="../../public/marketing-consultant-expert.jpg" alt="">
                        <h5>Richard Madsen</h5>
                        <p>Marketing Consulant Expert</p>
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
            </section>
        </div>
    </div>

</template>


<script>


</script>


<style>

section {
    position: relative;
    color: white
}

.padding-col {
    padding: 0 30px;
}

.bg-jumbo {
    background-image: url("../../public/marketing-intro.jpg");
    background-position: center;
    height: 700px;
}

.btn-white {
    padding: 8px 20px;
    border-style: none;
    border-radius: 8px;
    font-size: 14px;
}

.btn-white:hover {
    background: none;
    border: 1px solid white;
    color: white;
    font-size: 14px
}

.form-absolute {
    position: absolute;
    right: 300px;
    background-color: white;
    padding: 20px;
    border-radius: 8px;
}

.flex-form {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 10px
}

.img-rounded {
    width: 80px;
    height: 80px;
    border-radius: 50%;
}

.form-group {
    margin: 10px 0;
    width: 300px;
}

.condition-font {
    font-size: 10px;
    color: grey;
    text-align: center;
    margin-top: 10px;
}

.btn-orange-variant{
    background-color: #f76210;
    color: white;
    width: 100%;
    border-style: none;
    border-radius: 8px;
    padding: 8px 30px;
}


</style>