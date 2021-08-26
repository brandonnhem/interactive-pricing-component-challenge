<script>
	import Head from './Head.svelte';
	import Card from './Card.svelte';
</script>

<div class="top-bg"></div>
<div class="other-bg">
</div>

<Head/>

<Card/>

<footer>
	<div class="attribution">
		Challenge by <a href="https://www.frontendmentor.io/challenges/interactive-pricing-component-t0m8PIyY8">Frontend Mentor</a>. 
		Coded by <a href="https://github.com/brandonnhem">Brandon Nhem</a>.
	</div>
</footer>

<style>
	.attribution {
		font-size: 11px;
		text-align: center;
		margin-top: 8vh;
	}

	.attribution a {
		color: hsl(228, 45%, 44%);
	}

	.top-bg {
		position: absolute;
		background-color: hsl(222, 86.7%, 97.1%);
		width: 100%;
		height: 53%;
		z-index: -2;
		margin-left: -30px;
		margin-top: -30px;
		border-bottom-left-radius: 185px;
	}

	.other-bg {
		position: absolute;
		background-color: hsl(0, 0%, 100%);
		top: 32vh;
		margin-left: -30px;
		z-index: -3;
		height: 68%;
		width: 100%;
	}

	@media only screen and (min-width: 1440px) {
		.top-bg {
			height: 50vh;
			margin-left: -25vw;
			margin-top: -45vh;
			border-bottom-left-radius: 20% 50%;
		}

		.other-bg {
			top: 50vh;
			height: 67%;
			margin-left: -25vw;
		}
	}
</style>