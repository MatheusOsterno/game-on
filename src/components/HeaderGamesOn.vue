<template >
    <header>
        <nav class="container">
            <a href="/"><img src="../../public/logo gameson.png" alt="gameson" id="logo"></a>
            <img v-on:click="openMenu"  alt="abrir menu" id="menu-button" src="../assets/images/menu.svg">
            <div id="menu-overlay" v-if="menuActive" v-on:click="closeMenu"></div>
            <div id="menu-items" :class="{active:menuActive}">
                <img src="../../public/logo gameson.png" alt="gameson" id="menu-logo">
                <ul>
                    <li><a href="/">HOME</a></li>
                    <li><a href="/GAMES">GAMES</a></li>
                    <li><a href="/CONSOLES">CONSOLES</a></li>
                    <li><a href="/CONTATO">CONTATO</a></li>
                </ul>
            </div>
        </nav>
    </header>
</template>
<script>

export default {
    name:'HeaderGamesOn',
    data() {
        return {
            menuActive: false
        }
    },
    methods: {
            openMenu:  function() {
                this.menuActive = true;
            },
            closeMenu:  function() {
                this.menuActive = false;
            }
    },
}
</script>
<style scoped>
header {
    background-color: var(--color-background-nav);
    width: 100%;
    height: 60px;
    display: flex;
    justify-content: center;
    align-items: center;   
    box-shadow: rgba(9, 30, 66, 0.25) 0px 4px 8px -2px, rgba(9, 30, 66, 0.08) 0px 0px 0px 1px;}
#logo{

    width: 300px;
}
#menu-button {
    width: 30px;

}

nav{
    display: flex;
    justify-content: space-between;
    height: 60px;
    align-items: center;
}

#menu-overlay {
    position: fixed;
    top: 0;
    left: 0;
    width: 40%;
    height: 100vh;
    background-color: black;
    opacity: 0.8;
}

#menu-logo {
    width: 250px;
    margin-top: 30px;
    margin-bottom: 10px;
}

#menu-items {
    position: fixed;
    top: 0;
    right: 0;
    background-color: black;
    width: 60%;
    height: 100vh;
    display: none;
    flex-direction: column;
    justify-content: flex-start;
    align-items: center;
}

#menu-items.active {
    display: flex;
}

ul{
    list-style: none;
    text-align: center;
}

ul li {
    margin: 20px 0;
}

ul li a {
    color: white;
}

@media (min-width:700px) {
    #menu-button,
    #menu-logo,
    #menu-overlay {
        display: none;
    }

    #menu-items {
        color: white;
        display: flex;
        position: static;
        height: 60px;
        width: auto;
    }

    ul {
        display: flex;
        height: 60px;
        align-items: center;
    }
    ul li {
        margin: 0;
        margin-left: 20px;
    }
}
</style>