
<template>
    <div class="pokedex__container">
        <div class="pokedex__container__back-ground">
            <div class="pokedex__container__message">
                <img src="@/assets/logo_pokedex.png" alt="logo pokedex" class="pokedex__container__logo" />
            </div>
            <div class="pokedex__container__lupa">
                <form action="#" autocomplete="on">
                    <input class="pokedex__container__input__campo-busca" id="busca" name="busca" type="text"
                        placeholder="Nome do Pokemon">
                    <button type="submit" class="pokedex__container__input__btn-busca">
                        <i class="icon icon-search">
                            <svg xmlns="http://www.w3.org/2000/svg" height="24" viewBox="0 -960 960 960" width="24">
                                <path fill="white"
                                    d="M784-120 532-372q-30 24-69 38t-83 14q-109 0-184.5-75.5T120-580q0-109 75.5-184.5T380-840q109 0 184.5 75.5T640-580q0 44-14 83t-38 69l252 252-56 56ZM380-400q75 0 127.5-52.5T560-580q0-75-52.5-127.5T380-760q-75 0-127.5 52.5T200-580q0 75 52.5 127.5T380-400Z" />
                            </svg>
                        </i>
                    </button>
                </form>
            </div>
        </div>
    </div>
</template>
  
<style scoped>
.pokedex__container {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    height: 20vh;
    position: fixed;
}

.pokedex__container__back-ground {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 150px;
    background-color: #ff0000;
    background-position: left;
    background-size: 20%;
}

.pokedex__container__logo {
    padding-top: 2rem;
    height: 10rem;
    padding-left: 33%;
    padding-bottom: 2rem;
    position: fixed;
}

.pokedex__container__lupa {
    height: 100px;
    width: 20%;
    margin-left: 10px;
    position: fixed;
}

.pokedex__container__message {
    display: flex;
    justify-content: center;
    align-items: center;
    /* width: 30%; */
    padding-right: 25rem;
    position: fixed;
}

.pokedex__container__input__campo-busca,
.pokedex__container__input__campo-busca:focus {
    font-size: 35px;
    display: inline-block;
    font-family: 'open_sansregular';
    font-weight: 100;
    border: none;
    outline: none;
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
    position: fixed;
}

.pokedex__container__input__campo-busca:focus {
    width: 500px;
    z-index: 1;
    cursor: text;
    background-color: #ffffff;
    border-radius: 50px;
    padding: 0 25px;
    position: fixed;
}

.pokedex__container__input__btn-busca {
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
  