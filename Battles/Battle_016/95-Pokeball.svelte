<div class="main">
	<div class="top"></div>
	<div class="bottom"></div>
	<div class="middle"></div>
    <div class="circle"></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--green: #6cb3a9;
		--lightred: #d25b70;
		--white: #ffffff;
		--yellow: #f6df96;
		--red: #781728;
        background-color:var(--green);
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
	}

	.top,
	.bottom {
		position: absolute;
		height: 90px;
		width: 200px;
		background-color: transparent;
		/* opacity: 0.01; */
		transform: translateY(-55px);
		overflow: hidden;
		&:before {
			content: '';
			position: absolute;
			height: 200px;
			aspect-ratio: 1;
			background-color: var(--lightred);
			border-radius: 50%;
		}
		z-index: 1;
	}

	.bottom {
		transform: rotate(180deg) translateY(-55px);
		&:before {
			background-color: var(--white);
		}
	}

	.middle {
		position: absolute;
		height: 40px;
		width: 180px;
		background-color: var(--red);
		/* opacity: 0.1; */
		z-index: 0;
	}

    .circle{
        position:absolute;
        height:50px;
        aspect-ratio:1;
        border-radius:50%;
        z-index:3;
        /* opacity:0.7; */
        background-color:var(--yellow);
        box-shadow:0 0 0 10px var(--red);
    }
</style>
