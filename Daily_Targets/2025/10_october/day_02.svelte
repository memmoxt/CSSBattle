<div class="main">
	<div class="ear"></div>
	<div class="ear2"></div>
	<div class="head"></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--white: #fef6e2;
		--red: #ed736e;
		background-color: var(--white);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		position: absolute;
		& > div.ear,
		& > div.ear2 {
			position: absolute;
			height: 130px;
			width: 100px;
			background-color: var(--red);
			translate: -120px 55px;
			border-top-right-radius: 50px;
			border-top-left-radius: 75px;
			border-bottom-left-radius: 65px;
			border-bottom-right-radius: 65px;
		}
		& > div.ear2 {
			border-top-left-radius: 50px;
			border-top-right-radius: 75px;
			translate: 120px 55px;
		}
	}
	.head {
		position: absolute;
		height: 150px;
		width: 140px;
		translate: 0 -5px;
		background-color: var(--white);
		border-top-left-radius: 70px;
		border-top-right-radius: 70px;
		box-shadow: 0 0 0 40px var(--red);
		clip-path: polygon(-40px -40px, 180px -40px, 180px 150px, -40px 150px);
		&:before {
			content: '';
			position: absolute;
			height: 30px;
			width: 15px;
			background-color: var(--red);
			translate: 33px 65px;
			border-radius: 20px/40px;
			box-shadow: 60px 0 var(--red);
		}
	}
</style>
