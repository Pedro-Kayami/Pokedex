<template>
    <div class="pokedex">
        <div class="back-ground">
            <div class="header">
                <div class="mesage">
                    <img src="@/assets/logo_pokedex.png" alt="logo pokedex" class="logo" />
                </div>
                <div class="lupa">
                    <form action="#" autocomplete="on">

                        <input class="campo-busca" id="busca" name="busca" type="text" placeholder="Nome do Pokemon">
                        <button type="submit" class="btn-busca">
                            <i class="icon icon-search">
                                <svg xmlns="http://www.w3.org/2000/svg" height="24" viewBox="0 -960 960 960" width="24">
                                    <path fill="white"
                                        d="M784-120 532-372q-30 24-69 38t-83 14q-109 0-184.5-75.5T120-580q0-109 75.5-184.5T380-840q109 0 184.5 75.5T640-580q0 44-14 83t-38 69l252 252-56 56ZM380-400q75 0 127.5-52.5T560-580q0-75-52.5-127.5T380-760q-75 0-127.5 52.5T200-580q0 75 52.5 127.5T380-400Z" />
                                </svg> </i> </button>

                    </form>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
.header {
    display: flex;
    justify-content: flex-start;
    /* Alinha os itens à esquerda */
    align-items: center;
    width: 100%;
}

.pokedex {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    height: 100vh;
    /* background-color: #ffffff; */
    /* Altere para a cor que você deseja */
}

.back-ground {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 150px;
    background-color: #ff0000;
    background-position: left;
    background-size: 50%;
}

.logo {
    padding-top: 2.5rem;
    height: 10rem;
    padding-left: 80%;
    padding-bottom: 2.5rem;
    align-items: center;
}

.lupa {
    height: 100px;
    width: 20%;
    margin-left: 10px;
    /* Reduz a margem à esquerda */
}

.mesage {
    display: flex;
    justify-content: center;
    align-items: center;
    width: 100%;
    padding-right: 25rem;
}

.campo-busca {
    font-size: 35px;
    display: inline-block;
    font-family: 'open_sansregular';
    font-weight: 100;
    border: none;
    outline: none;
    /* color: #ffffff; */
    padding: 3px;
    padding-right: 50px;
    width: 0px;
    height: 50px;
    position: absolute;
    top: 0;
    right: 0;
    background: none;
    z-index: 3;
    transition: width .4s cubic-bezier(0.000, 0.795, 0.000, 1.000);
    cursor: pointer;
    margin-top: 3rem;
    margin-right: 20px;
}

.campo-busca:focus {
    width: 500px;
    z-index: 1;
    cursor: text;
    background-color: #007cff;
    border-radius: 50px;
    padding: 0 25px;
    margin-top: 3rem;
    margin-right: 20px;
}

.btn-busca {
    width: 50px;
    height: 50px;
    display: inline-block;
    color: white;
    font-size: 1.2em;
    float: right;
    border: none;
    border-radius: 50px;
    position: absolute;
    top: 0;
    right: 0;
    z-index: 2;
    cursor: pointer;
    background: #4c4c4c;
    margin-top: 3rem;
    margin-right: 20px;
}
</style>