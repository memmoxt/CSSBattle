<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--sky: #b0c1f0;
		--yellow: #fae29e;
		--blue: #3e5aa9;
        background-color: var(--sky);
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
			position: absolute;
			height: 80px;
			aspect-ratio: 1;
			background-color: var(--blue);
            box-shadow: 0 0 0 60px var(--yellow);
			&:before {
				content: '';
				position: absolute;
				height: 160px;
				aspect-ratio: 1;
				background-color: var(--blue);
				border-radius:50%;
				translate: -40px -40px;
				clip-path: polygon(
					0 35px,
					-50px 160px,
					55px 160px,
					55px 120px,
					120px 84px,
					160px 124px,
					160px 0px,
					106px 0px,
					106px 40px,
                    40px 40px,
                    40px 75px
				);
			}
		}
	}
</style>
