<template>
    <div class="container">
        <div class="flex">
        <img src="../../public/avada-marketing-logo-2x-200x37.png" alt="">

        <!-- ciclo per le voci della navbar -->
        <div>Ciao</div>

        <div>(555) 802-134</div>
        <button>Free Quote</button>
    </div>
    </div>

</template>


<script>
export default {
    name: 'TheHeader',
    data() {
        return {
        
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
    justify-content: space-around;
    padding: 20px;
    align-items: center;
}

button {
    border: 1px solid #ffe7da;
    background-color: #ffe7da;
    color: #f76210;
    padding: 5px 20px;
    border-radius: 10px;
}

button:hover {
    background-color: #f76210;
    color: white;
}



</style>