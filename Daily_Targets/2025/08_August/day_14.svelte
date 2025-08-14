<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		/* box-sizing: content-box; */
		box-sizing: border-box;
		--orange: #f3ac3c;
		--black: #000000;
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		position: absolute;
        background-color: var(--orange);
		& > div {
			height: 160px;
			aspect-ratio: 1;
			border-radius: 50%;
			translate: 0px -30px;
			&:before {
				content: '';
				position: absolute;
				background-color: var(--orange);
				translate: 40px 40px;
				height: 80px;
				border-radius: 50%;
				aspect-ratio: 1;
                box-shadow:0 0 0 40px var(--black);
                clip-path: polygon(-40px 40px, 160px 40px,160px 200px, -40px 200px);
			}
			&:after {
				content: '';
				position: absolute;
				height: 40px;
				aspect-ratio: 1;
				background-color: var(--black);
				border-radius: 50%;
				translate: 60px 60px;
                box-shadow: 60px 0 var(--black), -60px 0 var(--black), 0px 120px var(--black);
			}
		}
	}
</style>
