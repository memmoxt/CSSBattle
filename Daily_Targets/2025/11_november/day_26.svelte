<div class="main">
	<div></div>
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--purple: #62306d;
		--white: #ffffff;
        background-color:var(--purple);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		position: absolute;
		& > div:nth-child(1) {
			height: 280px;
			aspect-ratio: 1;
			background-color: var(--white);
			border-radius: 50%;
			translate: 0 20px;

			&:before {
				content: '';
				position: absolute;
				height: 80px;
				translate: 0 20px;
				border-radius: 50%;
				aspect-ratio: 1;
				background-color: var(--purple);
				translate: 100px 100px;
			}
			&:after {
				content: '';
				position: absolute;
				height: 110px;
				width: 400px;
				background-color: var(--purple);
				translate: -60px 160px;
				box-shadow: 0 0 0 20px var(--white);
			}
		}
		&>div:nth-child(2){
		    position:absolute;
		    height: 150px;
		    width:400px;
		    translate:0 95px;
		    clip-path:polygon(0px 100px, 80px 0px, 320px 0px, 400px 100px, 400px 130px, 0px 130px);
		    background-color:var(--purple);
            z-index: 3;
		}
		& > div:nth-child(3) {
			position: absolute;
            z-index: 2;
			height: 150px;
			width: 400px;
			translate: 0 95px;
			clip-path: polygon(0px 68px, 55px 0px, 346px 0px, 400px 68px, 400px 130px, 0px 130px);
			background-color: var(--white);
		}
	}
</style>
