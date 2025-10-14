<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--orange: #e8ad6d;
		--brown: #3b240c;
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
			position: absolute;
			height: 50px;
			width: 30px;
			background-color: var(--brown);
			translate: 0 60px;
			border-radius: 50px/50px;
			&:before {
				content: '';
				position: absolute;
				height: 160px;
				aspect-ratio: 1;
				background-color: var(--brown);
				border-radius: 50%;
				translate: -65px -130px;
				clip-path: polygon(0 90px, 160px 90px, 160px 160px, 0px 160px);
			}
			&:after {
				content: '';
				position: absolute;
				height: 100px;
				width: 60px;
				translate: -15px -120px;
				border-radius: 50px;
				box-shadow: 0 0 0 20px var(--orange);
				background-color: var(--brown);
			}
		}
	}
</style>
