<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--pink: #f1ddf5;
		--blue: #65a3c5;
		--black: #000000;
		--yellow: #eac049;
        background-color:var(--pink);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		flex-wrap: wrap;
		position: absolute;
		overflow: hidden;
		& > div {
			height: 30px;
			aspect-ratio: 1;
			background-color: black;
			/* opacity: 0.5; */
			border-radius: 50%;
			transform: translate(0px, -85px);
			box-shadow: 0 0 0 25px var(--yellow);
			&:before {
				content: '';
				position: absolute;
				height: 30px;
				aspect-ratio: 1;
				background-color: black;
				transform: translate(0px, 0px);
				border-radius: 50%;
				box-shadow: 0 0 0 25px var(--blue);
				clip-path: polygon(-25px -25px, 55px -25px, 55px 15px, -25px 15px);
			}
			&:after {
				content: '';
				position: absolute;
				height: 25px;
				aspect-ratio: 1;
				background-color: var(--blue);
				transform: translate(-25px, calc(25px / 2));
				box-shadow:
					0 25px 0 0 var(--blue),
					0 50px 0 0 var(--blue),
					0 78px 0 0 var(--black),
					0 55px 0 0 var(--blue),
					55px 178px 0 0 var(--black),
					55px 170px 0 0 var(--blue),
					55px 0 0 var(--blue),
					55px 25px 0 var(--blue),
					55px 50px 0 var(--blue),
					55px 75px 0 var(--blue),
					55px 100px 0 var(--blue),
					55px 125px 0 var(--blue),
					55px 150px 0 var(--blue);
			}
		}
	}
</style>

