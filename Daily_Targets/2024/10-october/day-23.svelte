<div class="main">
	<div></div>
	<div></div>
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--lightblue: #328fc1;
		--blue: #243d83;
		--yellow: #eeb850;
        background-color:var(--lightblue);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		& > div {
			position: absolute;
			height: 90px;
			aspect-ratio: 1;
			background-color:var(--blue) ;
			overflow: hidden;
			&:before {
				content: '';
				position: absolute;
				height: 90px;
				aspect-ratio: 1;
				background-color: var(--yellow);
				border-radius: 50%;
				transform: translateY(50%);
			}
		}
		& > div:nth-child(1) {
			transform: translate(-100%, 0%) rotate(-90deg);
		}
		& > div:nth-child(2) {
			transform: translate(100%, 0%) rotate(90deg);
		}
		& > div:nth-child(3) {
			transform: translate(0%, 100%) rotate(180deg);
		}
		& > div:nth-child(4) {
			transform: translate(0%, -100%);
		}
	}
</style>

