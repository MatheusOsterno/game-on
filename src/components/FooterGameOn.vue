<template lang="">
	<footer>
		<div class="main-content">
			<div class="left box">
				<h2> Sobre nós</h2>
				<div class="content">
					<p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Amet iste facilis harum eos vel incidunt distinctio corrupti iure? Rem</p>
				
					<div class="social">
						<a href="#"><span class="fab fa-facebook-f"></span></a>
						<a href="#"><span class="fab fa-twitter"></span></a>
						<a href="#"><span class="fab fa-instagram"></span></a>
						<a href="#"><span class="fab fa-youtube"></span></a>
					</div>
				</div>
			</div><!--left box-->
			<div class="center box">
				<h2>Endereço</h2>
				<div class="content">
					<div class="place">
						<span class="fas fa-map-marker"></span>
						<span class="text">Av.Brasil, Nova Capital</span>
					</div>

					<div class="phone">
						<span class="fas fas fa-phone-alt"></span>
						<span class="text">+55 61 9999-9999</span>
					</div>

					<div class="email">
						<span class="fas fa-envelope"></span>
						<span class="text">exemplo@exemplo.com</span>
					</div>
				</div>
			</div>
			<div class="right box">
				<h2>Contato</h2>
				<div class="content">
					<form action="#">
						<div class="email">
							<div class="text">Email *</div>
							<input type="email" required>
						</div>
						<div class="msg">
							<div class="text">Mensagem *</div>
							<textarea rows="2" cols="25" required></textarea>
						</div>
						<div class="btn">
							<button type="submit">Enviar</button>
						</div>
					</form>
				</div>
			</div>
		</div><!--main-content-->
		<div class="bottom">
			<div class="center">
				<span class="credit">Criado por Matheus Osterno <a href="#">FRONT</a></span>
				<span class="far fa-copyright">2022 Todos os diteitos reservados</span>
			</div>
		</div>
	</footer>

</template>
<script>
export default {
    
}
</script>
<style scoped>

*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    color: #d9d9d9;
    font-family: 'Poppins', sans-serif;
}
footer{
    bottom: 0px;
    width: 100%;
    background: black;
}
.main-content{
    display: flex;
}
.main-content .box{
    flex-basis: 50%;
    padding: 10px 20px;
}
.box h2{
    font-size: 18px;
    font-weight: 600;
    text-transform: uppercase;
}
.box .content{
    margin: 20px 0 0 0;
    position: relative;
}
.box .content:after{
    position: absolute;
    content: '';
    width: 15%;
    height: 2px;
    background: #f12020;
    top: -10px;
}
.box .content:before{
    position: absolute;
    content: '';
    height: 2px;
    width: 100%;
    background: #1a1a1a;
    top: -10px;
}
.left .content .social{
    margin: 20px 0 0 0;
}
.left .content .social a{
    padding: 0 2px;
}
.left .content .social a span{
    width: 40px;
    height: 40px;
    background: #1a1a1a;
    text-align: center;
    line-height: 40px;
    border-radius: 5px;
    font-size: 18px;
    transition: 0.3s;
}
.left .content .social a span:hover{
    background: #f12020;
}
.left .content p{
    text-align: justify;
}
.center .content .fas{
    font-size: 23px;
    background: #1a1a1a;
    width: 45px;
    height: 45px ;
    line-height: 45px;
    text-align: center;
    border-radius: 50%;
    transition: 0.3s;
    cursor: pointer;
}
.center .content .fas:hover{
    background: #f12020;
}
.center .content .text{
    font-size: 17px;
    font-weight: 500;
    padding-left: 10px;
}
.center .content .phone{
    margin: 10px 0;
}
.center .content .msg{
    margin-top: 10px;
}
.right form input, .right form textarea{
    width: 100%;
    font-size: 17px;
    background: #151515;
    padding-left: 10px;
    border: 1px solid #222222;
}
.right form input{
    height: 35px;
}
.right form input:focus,
.right form textarea:focus{
    outline-color: #3498db;
}
.right form .text{
    font-size: 17px;
    margin-bottom: 2px;
    color: #656565;
}
.right form .btn{
    margin-top: 10px;
}
.right form .btn button{
    height: 40px;
    width: 100%;
    background: #f12020;
    font-size: 17px;
    font-weight: 500;
    cursor: pointer;
    transition: .3s;
}
.right form .btn button:hover{
    background: #000;
}
.bottom .center{
    padding: 5px;
    font-size: 15px;
    background: #151515;
    text-align: center;
}
.bottom .center span{
    color: #656565;
}
.bottom .center a{
    color: #f12020;
    text-decoration: none;
}
.bottom .center a:hover{
    text-decoration: underline;
}
@media screen and (max-width: 900px){
    footer{
        bottom: 0px;
    }
    .main-content{
        flex-wrap: wrap;
        flex-direction: column;
    }
    .main-content .box{
        margin: 5px 0;
    }
}
    
</style>