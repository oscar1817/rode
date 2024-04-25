<script>
    //importamos el componente parImpar.svelte y lo llamamos parImpar
    import ParImpar from "./lib/parImpar.svelte";
    let valor = 0;
    //escuchamos el evento `input`
    const listenInput = (event) => (valor = event.target.avlue);
</script>

<main>
    <!--llamamos el componente ingresado un numero impar en este caso 5-->
    <ParImpar numero={5} />
    <!--llamamos nuevamente el componente ingresado un numero par en este caso 20-->
    <ParImpar numero={20} />
    <!--llamamos el componente ingresado un el número 0-->
    <ParImpar numero={0} />
</main>
