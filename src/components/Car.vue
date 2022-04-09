<template>
    <h2>Coche</h2>
    <p>Marca: {{ brand }}</p>
</template>

<script>
export default {

    setup(){
        const brand =  "Audi";
        const model =  "A4";
        const colors =  ["Azul","Morado", "Marron"];
        const price = 48000;
        const powers = [60,80,120,150,200,220,300,385,480,625];
        const mensaje = {
            title: "Estoy bien",
            text: "Welcome",
        };

        return {
            brand,
            model,
            colors,
            price,
            power,
            mensaje,
        };
    },

};
</script>

<style>

</style>