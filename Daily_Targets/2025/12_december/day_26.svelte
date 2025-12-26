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
		--purple: #a82973;
		--pink: #eec8ea;
        background-color: var(--purple);
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
			height: 60px;
			aspect-ratio: 1;
			background-color: var(--pink);
			transform: translate(-40px, 40px) rotate(10deg);
		}
		& > div:nth-child(2) {
			translate: -16px -91px;
			rotate: -20deg;
		}
		& > div:nth-child(3) {
			translate: 80px -80px;
			rotate: 0deg;
		}
        &>div:nth-child(4){
            translate: 64px -11px;
			rotate: -20deg;
        }
	}
</style>
