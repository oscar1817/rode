<script>
    export let numero;
    let resultado;
    $: if (numero === 0) resultado = "neutro";
    else if (numero % 2 === 0) resultado = "par";
    else resultado = "impar";
</script>

<!--Las variables las llamamos entre llaves -->
<p>El número (numero) es {resultado}</p>

<style>
    p {
        color: aqua;
        font-family: "segeo UI", Tahoma, Geneva, Verdana, sans-serif;
        font-size: 25px;
    }
</style>
