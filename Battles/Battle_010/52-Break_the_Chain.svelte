<div class="main">
    <div class="big-ball"></div>
	<div class="grid-a">
		<div></div>
		<div></div>
		<div></div>
	</div>
	<div class="grid-b">
		<div></div>
		<div></div>
		<div></div>
		<div></div>
	</div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--yellow: #eeb850;
		--light-blue: #6592cf;
		--blue: #243d83;
	}

	.main {
		height: 300px;
		width: 400px;
		display: grid;
		grid-template-columns: 28px 135px 30px 180px;
		align-items: center;
        background-color:var(--light-blue);
        &>.big-ball{
            position:absolute;
            height:60px;
            aspect-ratio:1;
            border-radius:50%;
            background-color:var(--yellow);
            transform:translate(65px, -20px);
        }
		& > .grid-a {
			display: grid;
			grid-template-columns: repeat(3, 1fr);
			grid-column: 2;
			height: 80px;
			width: 135px;
			justify-items: center;
			align-items: end;
			& > div {
				height: 40px;
				aspect-ratio: 1;
				border-radius: 50%;
				background-color: var(--yellow);
                transform:translate(0px, -30px);
				&:before {
					content: '';
					position: absolute;
					height: 20px;
					aspect-ratio: 1;
					border-radius: 50%;
                    transform:translate(10px, 10px);
					background-color: var(--blue);
				}
				&:after {
					content: '';
					position: absolute;
					height: 50px;
					width: 10px;
                    transform:translate(15px, 20px);
					background-color: var(--blue);
				}
			}
		}
		& > .grid-b {
			display: grid;
			grid-template-columns: repeat(4, 1fr);
			grid-column: 4;
			justify-items: center;
			align-items: end;
			height: 80px;
			width: 180px;
			& > div {
				height: 50px;
				width: 10px;
				background-color: var(--blue);
				&:before {
					content: '';
					position: absolute;
					height: 20px;
					aspect-ratio: 1;
					border-radius: 50%;
					background-color: var(--blue);
					transform: translate(-25%, -50%);
				}
			}
		}
	}
</style>

