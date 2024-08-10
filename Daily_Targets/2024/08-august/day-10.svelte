<div class="main">
	<div>
		<div></div>
	</div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--white: #eadcdc;
		--blue: #3166ae;
		background-color: var(--white);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		& > div {
			height: 140px;
			aspect-ratio: 1;
			background-color: var(--blue);
			border-radius: 50%;
			overflow: hidden;

			&:before {
				content: '';
				position: absolute;
				background-color: var(--white);
				height: 50px;
				width: 50px;
				transform: translate(45px, 30px);
				border-radius: 50%;
				clip-path: polygon(0 0, 50px 0px, 50px 21px, 0px 21px);
			}
			&:after {
				content: '';
				position: absolute;
				background-color: var(--white);
				height: 50px;
				width: 50px;
				border-radius: 50%;
				transform: translate(45px, 45px);
				clip-path: polygon(0px 21px, 50px 21px, 50px 50px, 0px 50px);
			}
			& > div {
				height: 15px;
				width: 70px;
				transform: translate(82px, 81px);
				background-color: var(--white);
			}
		}
	}
</style>

