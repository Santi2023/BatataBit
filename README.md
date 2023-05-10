# BatataBit
Pagina responsive de la criptomoneda batatabit
/* 
1. Posicionamiento
2. Modelo caja (Box model)
3. Tipografía
4. Visuales
5. Otros
*/

:root {
    /* Colores */
    --bitcoin-orange: #f7931A;
    --soft-orange: #ffe9D5;
    --secondary-blue: #1a9af7;
    --soft-blue: #e7f5ff;
    --warm-black: #201e1c;
    --black: #282623;
    --gray: #bababa;
    --off-white: #faf8f7;
    --just-white: #ffffff;
}

* {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}

html {
    font-size: 62.5%;
    font-family: 'DM Sans', sans-serif;
    scroll-behavior: smooth;
    /* font-family: 'Inter', sans-serif; */
}

header {
    position: relative;
    display: flex;
    flex-direction: column;
    justify-content: center;
    width: 100%;
    min-width: 320px;
    height: 334px;
    align-items: center;
    background: linear-gradient(207.8deg, #201E1C 16.69%, #F7931A 100%);
}

header img {
    width: 150px;
    height: 24px;
    margin-top: 60px;
    align-self: center;
}

.header--title-container {
    width: 90%;
    min-width: 288px;
    max-width: 900px;
    height: 218px;
    margin-top: 40px;
    text-align: center;
}

.header--title-container h1 {
    font-size: 2.4rem;
    font-weight: bold;
    line-height: 2.6rem;
    color: var(--just-white);
}

.header--title-container p {
    margin-top: 25px;
    font-size: 1.4rem;
    font-weight: 500;
    line-height: 1.8rem;
    color: var(--soft-orange);
}

.header--title-container .header--button {
    position: absolute;
    left: calc(50% - 118px);
    top: 270px;
    display: block;
    margin-top: 35px;
    padding: 15px;
    width: 229px;
    height: 48px;
    background-color: var(--off-white);
    /* Sombreado */
    box-shadow: 0px 4px 8px rgba(89, 73, 30, 0.16);
    border: none;
    border-radius: 5px;
    font-size: 1.4rem;
    font-weight: bold;
    text-decoration: none;
    color: var(--black);
}

.header--button span {
    display: inline-block;
    width: 13px;
    height: 8px;
    margin-left: 10px;
    background-image: url('./assets/icons/down-arrow.svg');
}

main {
    width: 100%;
    height: auto;
    background-color: var(--off-white);
}

.main-exchange-container {
    width: 100%;
    height: auto;
    padding-top: 80px;
    padding-bottom: 30px;
    text-align: center;
}

.main-exchange-container--title {
    width: 90%;
    min-width: 288px;
    max-width: 900px;
    margin: 0 auto;
}

.main-exchange-container .backgroundImg {
    width: 200px;
    height: 200px;
    margin: 0 auto;
    margin-bottom: 50px;
    background-image: url('./assets/img/Bitcoin.svg');
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;
}

.main-exchange-container h2 {
    margin-bottom: 30px;
    font-size: 2.4rem;
    font-weight: bold;
    line-height: 2.6rem;
    color: var(--black);
}

.main-exchange-container p {
    margin-bottom: 30px;
    font-size: 1.4rem;
    font-weight: 500;
    line-height: 1.6rem;
    color: #757575;
}

.main-tables-container {
    display: flex;
    margin: 0 calc(50% - 120px) 0;
    height: 380px;
    overflow-x: scroll;
    overscroll-behavior-x: contain;
    scroll-snap-type: x proximity;
}

.main-tables-container::-webkit-scrollbar {
    height: 8px;
    width: 10px;
}

.main-tables-container::-webkit-scrollbar-thumb {
    background-color: #F7CE68;
    border-radius: 10px;
}

.main-tables-container::-webkit-scrollbar-track{
    background-color: var(--soft-orange);
}

.main-currency-table {
    scroll-snap-align: center;
    width: 70%;
    min-width: 235px;
    max-width: 500px;
    height: 360px;
    margin: 0 auto;
    font-family: 'Inter', sans-serif;
}

.main-currency-table .currency-table--title {
    margin-bottom: 15px;
    font-size: 1.8rem;
    font-weight: bold;
    line-height: 2.3rem;
}

.main-currency-table .moneda {
    color: var(--bitcoin-orange);
}

.main-currency-table .comision {
    color: var(--secondary-blue);
}

.currency-table--container {
    width: 90%;
    min-width: 230px;
    max-width: 300px;
    height: 250px;
    margin: 0 auto;
}

.currency-table--container table {
    width: 100%;
    height: 100%;
}

.currency-table--container td {
    width: 50%;
    font-size: 1.6rem;
    font-weight: 500;
    line-height: 1.9rem;
    color: var(--gray);
    background-color: var(--just-white);
}

.currency-table--container .table__top-left {
    border-radius: 15px 0 0 0;
}

.currency-table--container .table__top-right {
    border-radius: 0 15px 0 0;
}

.currency-table--container .table__bottom-left {
    border-radius: 0 0 0 15px;
}

.currency-table--container .table__bottom-right {
    border-radius: 0 0 15px 0;
}

.currency-table--container .table__right {
    font-size: 1.4rem;
    font-weight: normal;
    line-height: 1.7rem;
    color: #757575;
}

.currency-table--container .trending {
    display: inline-block;
    width: 15px;
    height: 15px;
    margin-left: 10px;
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;
}

.currency-table--container .down {
    background-image: url('./assets/icons/trending-down.svg');
}

.currency-table--container .up {
    background-image: url('./assets/icons/trending-up.svg');
}

.currency-table--date {
    width: 190px;
    height: 30px;
    margin: 0 auto;
    margin-top: 15px;
    padding: 8px;
    border-radius: 8px;
}

.date-money {
    background-color: var(--soft-orange);
}

.date-comision {
    background-color: var(--soft-blue);
}

.currency-table--date p {
    font-size: 1.2rem;
    font-weight: 300;
    line-height: 1.5rem;
    color: var(--warm-black);
}

.main-product-detail {
    position: relative;
    width: 100%;
    min-width: 320px;
    height: auto;
    padding: 20px 10px;
    background-color: var(--warm-black);
}

.product-detail--batata-logo {
    position: absolute;
    width: 40px;
    height: 25px;
    top: -10px;
    left: calc(50% - 20px);
    background-image: url('./assets/icons/batata.svg');
}

.product-detail--title {
    width: 90%;
    min-width: 288px;
    height: auto;
    margin: 0 auto;
    margin-top: 50px;
    text-align: center;
}

.product-detail--title h2 {
    margin-bottom: 20px;
    font-size: 2.4rem;
    font-weight: bold;
    line-height: 2.6rem;
    color: var(--just-white);
}

.product-detail--title p {
    margin-bottom: 20px;
    font-size: 1.4rem;
    font-weight: 500;
    line-height: 1.8rem;
    color: #808080;
}

.product-detail--card {
    width: 90%;
    min-width: 288px;
    max-width: 400px;
    height: 150px;
    margin: 15px auto;
    padding: 15px;
    background-color: var(--black);
    border-radius: 5px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.16);
}

.product-detail--card .icon-card {
    display: inline-block;
    width: 20px;
    height: 20px;
    margin-bottom: 10px;
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;
}

.clock {
    background-image: url('./assets/icons/clock.svg');
}

.eye {
    background-image: url('./assets/icons/eye.svg');
}

.dollar {
    background-image: url('./assets/icons/dollar-sign.svg');
}

.check-circle {
    background-image: url('./assets/icons/check-circle.svg');
}

.product--card-title {
    margin-bottom: 15px;
    font-size: 1.8rem;
    font-weight: bold;
    line-height: 1.8rem;
    color: var(--just-white);
}

.product--card-body {
    font-size: 1.4rem;
    font-weight: 500;
    line-height: 1.8rem;
    color: #808080;
    text-align: center;
}

.bitcoin-img-container {
    width: 100%;
    min-width: 320px;
    height: 50vh;
    background-image: url('./assets/img/bitcoinbaby2x.jpg');
    background-position: center;
    background-size: cover;
    background-repeat: no-repeat;
    text-align: center;
}

.bitcoin-img-container h2 {
    padding-top: 60px;
    font-size: 2.4rem;
    font-weight: bold;
    line-height: 2.6rem;
    color: var(--just-white);
}

.main-plans-container {
    width: 100%;
    min-width: 320px;
    padding-bottom: 70px;
    text-align: center;
    background-color: var(--off-white);
}

.plans--title {
    width: 90%;
    min-width: 288px;
    height: auto;
    margin: 0 auto;
    margin-bottom: 50px;
}

.plans--title h2 {
    padding-top: 50px;
    font-size: 2.4rem;
    font-weight: bold;
    line-height: 2.6rem;
    color: var(--black);
}

.plans--title p {
    padding-top: 30px;
    font-size: 1.4rem;
    font-weight: 500;
    line-height: 1.8rem;
    color: #757575;
}

.plans-container--slider {
    display: flex;
    height: 316px;
    overflow-x: scroll;
    overscroll-behavior-x: contain;
    scroll-snap-type: x proximity;
}

.plans-container--slider::-webkit-scrollbar {
    height: 8px;
    width: 10px;
}

.plans-container--slider::-webkit-scrollbar-thumb {
    background-color: #F7CE68;
    border-radius: 10px;
}

.plans-container--slider::-webkit-scrollbar-track {
    background-color: var(--soft-orange);
}

.plans-container--card {
    position: relative;
    scroll-snap-align: center;
    width: 70%;
    min-width: 190px;
    max-width: 300px;
    height: 250px;
    margin: 50px 5px 0;
    padding: 0 15px;
    background-color: var(--just-white);
    border-radius: 15px;
    box-shadow: 0 4px 8px rgba(89, 73, 30, 0.16);
}

.plans-container--card:nth-child(3){
    background-color: var(--warm-black);
}

.card-etiqueta {
    position: absolute;
    width: 120px;
    height: 31px;
    left: calc(50% - 60px);
    top: -15px;
    padding: 6px;
    font-size: 1.2rem;
    border-radius: 8px;
    color: var(--just-white);
}

.basic {
    background-color: var(--secondary-blue);
}

.recomended {
    background-color: var(--bitcoin-orange);
 
}

.unilimited {
    background-color: var(--black);
    color: var(--bitcoin-orange);
    border: 1px solid var(--bitcoin-orange);
}

.plan-card--title {
    padding-top: 30px;
    font-size: 1.4rem;
    font-weight: 500;
    line-height: 1.8rem;
    color: black;
}

.plan-card--price {
    padding: 8px 0;
    font-size: 5.2rem;
    font-weight: bold;
    line-height: 5.3rem;
    color: black;
}


.plan-card--price sup {
    vertical-align: top;
    font-family: “Inter”, sans-serif;
    font-size: 1.2rem;
    font-weight: 300;
    line-height: 1.5rem;
    color: var(--gray)
}

.plan-card--price span {
    vertical-align: top;
    font-family: “Inter”, sans-serif;
    font-size: 1.2rem;
    font-weight: 300;
    line-height: 1.5rem;
    color: var(--gray)
}

.plan-card--saving {
    font-size: 1.2rem;
    color: #757575;
}

.color-unilimited {
    color: var(--just-white);
}

.plan-card--ca {
    width: 150px;
    height: 48px;
    margin-top: 20px;
    background-color: var(--off-white);
    border: 2px solid var(--bitcoin-orange);
    border-radius: 4px;
    font-family: 'DM Sans', sans-serif;
    font-size: 1.4rem;
    font-weight: bold;
    line-height: 1.8rem;
    color: var(--warm-black);
}

.ca-unilimited {
    background-color: var(--black);
    color: var(--just-white);
}

.plan-card--ca:hover {
    background-color: var(--soft-orange);
}

.plan-card--ca span {
    display: inline-block;
    width: 20px;
    height: 20px;
    background-image: url('./assets/icons/orange-right-arrow.svg');
    vertical-align: text-bottom;
}

footer {
    display: flex;
    width: 100%;
    height: 150px;
    background-color: var(--bitcoin-orange);
}

footer section {
    width: 50%;
    display: flex;
    justify-content: center;
    align-items: center;
}

.footer-section-left ul {
    font-size: 1.4rem;
    font-weight: 500;
    line-height: 1.8rem;
    list-style: none;
}

.footer-section-left li {
    margin: 10px 0;
}

.footer-section-left a {
    text-decoration: none;
    color: var(--just-white);
}

.footer-section-right img {
    width: 85px;
    width: 85px;
}

<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <link rel="stylesheet" href="./style.css">
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link
        href="https://fonts.googleapis.com/css2?family=DM+Sans:wght@400;500;700&family=Inter:wght@300;500&display=swap"
        rel="stylesheet">
</head>

<body>
    <header>
        <img src="./assets/img/logo.svg" alt="logo">
        <div class="header--title-container">
            <h1>La próxima revolución en el intercambio de criptomonedas.</h1>
            <p>Batatabit te ayuda a navegar entre los diferentes precios y tendencias.</p>
            <a href="#plans" class="header--button">Conoce Nuestros Planes <span></span></a>
        </div>
    </header>
    <main>
        <section class="main-exchange-container">
            <div class="backgroundImg"></div>
            <div class="main-exchange-container--title">
                <h2>Visibilizamos todas las tasas de cambio.</h2>
                <p>Traemos información en tiempo real de las casas de cambio y las monedas más importantes del mundo.
                </p>
            </div>
            <section class="main-tables-container">
                <div class="main-currency-table">
                    <p class="currency-table--title moneda">Monedas</p>
                    <div class="currency-table--container">
                        <table>
                            <tr>
                                <td class="table__top-left">Bitcoin</td>
                                <td class="table__top-right table__right">$ 1.96 <span class="trending down"></span>
                                </td>
                            </tr>
                            <tr>
                                <td>Ethereum</td>
                                <td class="table__right">$ 0.07 <span class="trending up"></span></td>
                            </tr>
                            <tr>
                                <td>Ripple</td>
                                <td class="table__right">$ 2.17 <span class="trending down"></span></td>
                            </tr>
                            <tr>
                                <td class="table__bottom-left">Stellar</td>
                                <td class="table__bottom-right table__right">$ 4.96 <span class="trending down"></span>
                                </td>
                            </tr>
                        </table>

                    </div>
                    <div class="currency-table--date date-money">
                        <p>
                            <b>Actualizado:</b> 08 Mayo 23:45
                        </p>
                    </div>
                </div>
                <div class="main-currency-table">
                    <p class="currency-table--title comision">Comisiones</p>
                    <div class="currency-table--container">
                        <table>
                            <tr>
                                <td class="table__top-left">Bitrade</td>
                                <td class="table__top-right table__right">$ 12.96</td>
                            </tr>
                            <tr>
                                <td>Bitpreco</td>
                                <td class="table__right">$ 13.07</td>
                            </tr>
                            <tr>
                                <td>Novadax</td>
                                <td class="table__right">$ 13.15</td>
                            </tr>
                            <tr>
                                <td class="table__bottom-left">Coinext</td>
                                <td class="table__bottom-right table__right">$ 14.96</td>
                            </tr>
                        </table>

                    </div>
                    <div class="currency-table--date date-comision">
                        <p>
                            <b>Actualizado:</b> 08 Mayo 23:45
                        </p>
                    </div>
                </div>
            </section>
        </section>
        <section class="main-product-detail">
            <span class="product-detail--batata-logo"></span>
            <div class="product-detail--title">
                <h2>Creamos un producto sin comparación.</h2>
                <p>Confiable y diseñado para su uso diario.</p>
            </div>
            <section class="product-cards--container">
                <article class="product-detail--card">
                    <span class="icon-card clock"></span>
                    <p class="product--card-title">Tiempo real</p>
                    <p class="product--card-body">Nuestro API toma información minuto a minuto sobre las tasas que más
                        determinan el comportamiento.</p>
                </article>
                <article class="product-detail--card">
                    <span class="icon-card eye"></span>
                    <p class="product--card-title">No hay tasas escondidas</p>
                    <p class="product--card-body">Ni en la compra o al momento de exit, Batabit siempre te muestra el
                        costo real de lo que estás adquiriendo.</p>
                </article>
                <article class="product-detail--card">
                    <span class="icon-card dollar"></span>
                    <p class="product--card-title">Compara monedas</p>
                    <p class="product--card-body">Ni en la compra o al momento de exit, Batabit siempre te muestra el
                        costo real de lo que estás adquiriendo.</p>
                </article>
                <article class="product-detail--card">
                    <span class="icon-card check-circle"></span>
                    <p class="product--card-title">Información confiable</p>
                    <p class="product--card-body">Nuestras fuentes están 100% verificadas y continuamos auditando su
                        contenido mientras se actualizan.</p>
                </article>
            </section>
        </section>
        <section class="bitcoin-img-container">
            <h2>Conócelo hoy.</h2>
        </section>
        <section id="plans" class="main-plans-container">
            <div class="plans--title">
                <h2>Escoge el plan que mejor se ajuste a ti.</h2>
                <p>Cualquier plan te da acceso completo a nuestra plataforma.</p>
            </div>
            <section class="plans-container--slider">
                <article class="plans-container--card">
                    <p class="card-etiqueta basic">Basico</p>
                    <div class="plans-info-container">
                        <h3 class="plan-card--title">Pago Anual</h3>
                        <p class="plan-card--price"><sup>$</sup>5</p>
                        <p class="plan-card--saving">*Plan básico para mantenerte informado</p>
                        <button class="plan-card--ca">Escoger este <span></span></button>
                    </div>
                </article>
                <article class="plans-container--card">
                    <p class="card-etiqueta recomended">Recomendado</p>
                    <div class="plans-info-container">
                        <h3 class="plan-card--title">Pago Anual</h3>
                        <p class="plan-card--price"><sup>$</sup>49</p>
                        <p class="plan-card--saving">*Ahorras $129 comparado al plan mensual.</p>
                        <button class="plan-card--ca">Escoger este <span></span></button>
                    </div>
                </article>
                <article class="plans-container--card">
                    <p class="card-etiqueta unilimited">Unilimite</p>
                    <div class="plans-info-container">
                        <h3 class="plan-card--title color-unilimited">Acceso de por vida</h3>
                        <p class="plan-card--price color-unilimited"><sup>$</sup>99</p>
                        <p class="plan-card--saving color-unilimited">*Ahorras $999+ comparado al plan anual.</p>
                        <button class="plan-card--ca ca-unilimited">Escoger este <span></span></button>
                    </div>
                </article>
            </section>
        </section>
    </main>
    <footer>
        <section class="footer-section-left">
            <ul>
                <li><a href="#">Linkedin</a></li>
                <li><a href="#">Crunchbase</a></li>
                <li><a href="#">Hackernews</a></li>
            </ul>
        </section>
        <section class="footer-section-right">
            <img src="./assets/img/logo-footer.svg" alt="Logo de Batatabit 2020">
        </section>
    </footer>
</body>

</html>
