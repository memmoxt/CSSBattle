<div class="main">
	<div class="clock"></div>
	<div class="clock"></div>
	<div class="clock"></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--purple: #492fb0;
		--pink: #db5ead;
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
	}
	.clock {
		position: absolute;
		translate: -130px;
		height: 150px;
		width: 50px;
		background-color: var(--pink);

		&:before {
			content: '';
			position: absolute;
			height: 100px;
			aspect-ratio: 1;
			background-color: var(--pink);
			border-radius: 50%;
			translate: -25px 25px;
		}
	}
	.clock:nth-child(2) {
		translate: 0px;
        transform: rotate(15deg);
	}
    .clock:nth-child(3){
		translate: 130px;
        transform: rotate(30deg);
    }
</style>
