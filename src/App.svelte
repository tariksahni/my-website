<script>
	import Home from 'Screens/home';
	import Header from 'Screens/header';
</script>

<style>
	:global(body){
		height: 100vh;
		width: 100vw;
		background-color: #111;
		padding: 0;
		overflow: hidden;
		font-size: 10px;
	}
	:global(.poppins-font){
		font-family: 'Poppins', sans-serif;
	}
	:global(.open-sans-font){
		font-family: 'Open Sans', sans-serif;
	}
	:global(.yellow-color){
		color: #ffb400;
	}
	:global(.white-color){
		color: #fff;
	}
	:global(.upper-case){
		text-transform: uppercase;
	}
	:global(.yellow-color-background){
		background-color: #ffb400;
	}
	@media (max-width: 991px)  {
		:global(.fs-2){
			font-size: 16px;
		}
		:global(.fs-3){
			font-size: 16px;
		}
		:global(.fs-4){
			font-size: 24px;
		}
		:global(.fs-5){
			font-size: 32px;
		}
		:global(.fs-6){
			font-size: 48px;
		}
	}
	@media (min-width: 991px) {
		:global(.fs-1) {
			font-size: 8px;
		}

		:global(.fs-2) {
			font-size: 16px;
		}

		:global(.fs-3) {
			font-size: 24px;
		}

		:global(.fs-4) {
			font-size: 32px;
		}

		:global(.fs-5) {
			font-size: 48px;
		}
	}
	:global(.fw-normal){
		font-weight: normal;
	}
	:global(.fw-medium){
		font-weight: 500;
	}
	:global(.fw-bold){
		font-weight: 600;
	}

</style>

<Home />
<Header />
