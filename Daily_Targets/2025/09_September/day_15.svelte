<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--white: #fff1f1;
		--red: #f2a3ab;
		--blue: #84b9c7;
        background-color:var(--white);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		position: absolute;
		& > div {
			height: 180px;
			width: 50px;
			translate: -115px;
			background-color: var(--red);
			box-shadow: 230px 0 var(--red);
			&:before {
				content: '';
				position: absolute;
				height: 80px;
				aspect-ratio: 1;
				border-radius: 50%;
				translate: 145px 50px;
				box-shadow: 0 0 0 50px var(--blue);
				clip-path: polygon(-50px -50px, 40px -50px, 40px 130px, -50px 130px);
				background-color: var(--white);
			}
		}
	}
</style>
