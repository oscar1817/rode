<script>
    export let pais;
    let p;
    /*[0]-Nombre_pais [1]-capital [2]-poblacion [3]-moneda [4]-área [5]-bandera*/
    const paises = {
        colombia: [
            "Colombia",
            "Bogota",
            "51,52 millones",
            "Peso colombiano",
            "1,142 millones km2",
            "Flag_of_Colombia.svg",
        ],
        venezuela: [
            "Venezuela",
            "Caracas",
            "28,2 millones",
            "Bolivar",
            "916.445 km2",
            "Flag_of_Venezuela.svg",
        ],
        ecuador: [
            "Ecuador",
            "Quito",
            "17,8 millones",
            "Dólar estadounidense",
            "256.370 km2",
            "Flag_of_Ecuador.svg",
        ],
        peru: [
            "Peru",
            "Lima",
            "33,72 millones",
            "Sol peruano",
            "1.285.215 km2",
            "Flag_of_peru.svg",
        ],
        brasil: [
            "Brasil",
            "Brasilia",
            "214,3 millones",
            "Real brasileño",
            "8.51 millones km2",
            "Flag_of_Brazil.svg",
        ],
        argentina: [
            "Argentina",
            "Buenos aires",
            "45 millones",
            "Peso argentino",
            "2.780.400 km2",
            "Flag_of_argentina.svg",
        ],
        paraguay: [
            "Paraguay",
            "Asuncion",
            "6,109,644 millones",
            "Guarani",
            "15.02 km2",
            "Flag_of_paraguay.svg",
        ],
        uruguay: [
            "Uruguay",
            "Montevideo",
            "3,444,263 millones",
            "Uruguayan peso",
            "19.5 km2",
            "Flag_of_uruguay.svg",
        ],
        bolivia: [
            "Bolivia",
            "Sucre",
            "12,186,073 millones",
            "Boliviano",
            "11.09 km2",
            "Flag_of_bolivia.svg",
        ],
        chile: [
            "Chile",
            "Santiago",
            "2,423,263 millones",
            "Peso chileno",
            "756.626 km2",
            "Flag_of_chile.svg",
        ],
    };
    p = paises[pais];
</script>

<div class="main">
    <div class="col1">
        <img
            src="./src/assets/{p[5]}"
            alt="Bandera_Colombia"
            width="300"
            height="200"
        />
    </div>
    <div class="col2">
        <div class="linea"><strong>Pais:</strong> {p[0]}</div>
        <div class="linea"><strong>Capital:</strong> {p[1]}</div>
        <div class="linea"><strong>Poblacion:</strong> {p[2]}</div>
        <div class="linea"><strong>Moneda:</strong> {p[3]}</div>
        <div class="linea"><strong>Extension:</strong> {p[4]}</div>
    </div>
</div>

<style>
    .main {
        display: grid;
        grid-template-columns: repeat(4, 1fr);
        grid-gap: 5px;
        grid-auto-rows: minmax(100px, auto);
        border-radius: 10px;
        border-style: solid;
        border-color: blue;
        border-width: 2px;
        margin: left;
        width: 600px;
        box-shadow: 5px 5px 5px rgb(0, 157, 255);
        margin-right: 5px;
        margin-bottom: 10px;
    }
    .col1 {
        grid-column: 1;
        grid-row: 1;
        margin: 5px;
        padding: 5px;
    }
    .col2 {
        grid-column: 2;
        grid-row: 1;
        margin: 5px;
        padding: 5px;
        border-color: brown;
        width: max-content;
    }
    strong {
        color: rgb(0, 17, 255);
        font-weight: bolder;
    }
    .linea {
        font-size: 20px;
        margin-bottom: 18px;
    }
</style>
