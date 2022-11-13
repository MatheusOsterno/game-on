<template>
    <section class="container">
        <div class="card">
            <div class="card-image game1"></div>
            <h2>Game 1</h2>
            <p>Lorem Ipsum is and scrambleesf Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.</p>
            <a href="/">Leia mais</a>
        </div>
        <div class="card">
            <div class="card-image game2"></div>
            <h2>Game 2</h2>
            <p>Lorem Ipsum is and scrambleesf Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.</p>
            <a href="/">Leia mais</a>
        </div>
        <div class="card">
            <div class="card-image game3"></div>
            <h2>Game 3</h2>
            <p>Lorem Ipsum is and scrambleesf Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.</p>
            <a href="/">Leia mais</a>
        </div>
        <div class="card">
            <div class="card-image game1"></div>
            <h2>Game 1</h2>
            <p>Lorem Ipsum is and scrambleesf Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.</p>
            <a href="/">Leia mais</a>
        </div>
        <div class="card">
            <div class="card-image game2"></div>
            <h2>Game 2</h2>
            <p>Lorem Ipsum is and scrambleesf Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.</p>
            <a href="/">Leia mais</a>
        </div>
        <div class="card">
            <div class="card-image game3"></div>
            <h2>Game 3</h2>
            <p>Lorem Ipsum is and scrambleesf Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.</p>
            <a href="/">Leia mais</a>
        </div>
    </section>
</template>
<script>
export default {
    
}
</script>
<style scoped>
.container {
    margin: auto;
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
}

.card {
    background: black;
    color: white;
    width: 270px;
    height: 450px;
    margin: 10px;
    border-radius: 15px;
    margin-top: 30px;
    margin-bottom: 30px;
}

.card-image {
    height: 150px;
    margin-bottom: 15px;
    border-radius: 15px 15px 0 0;
    background-size: cover;
}

.card p {
    padding: 10px;
}

.card h2 {
    padding: 10px;
}

.card a {
    background-color: #058905;
    color: white;
    padding: 15px 20px ;
    display: block;
    text-align: center;
    margin: 20px 50px;
}

.game1 {
    background-image: url('https://s2.glbimg.com/U-djrmeL0Mmhr1rjtn5hVAPRu88=/0x0:1920x1080/1008x0/smart/filters:strip_icc()/i.s3.glbimg.com/v1/AUTH_08fbf48bc0524877943fe86e43087e7a/internal_photos/bs/2019/J/f/IY697dSgejr3wbPYLA8w/dmc1.jpg');
    height: 150px;
}

.game2 {
    background-image: url('https://image.api.playstation.com/vulcan/img/rnd/202201/2122/f9rMmCsm9C54dpvUKVqSX29L.jpg');
    height: 150px;
}
.game3 {
    background-image: url('https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRU4YrUoxTKGA1nNniUzBERqZXgJk6DmDD61w&usqp=CAU');
    height: 150px;
}

.card:hover {
    background-color: #058905;
    transform: scale(1.03);
    transition: all 1s ease;
}
</style>