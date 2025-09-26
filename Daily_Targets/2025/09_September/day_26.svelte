<div class="main">
	<div>
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
		--blue: #4763b1;
		--white: #ffffff;
		--black: #000000;
        background-color:var(--blue);
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
			position: relative;
			height: 200px;
			width: 200px;
			display: grid;
			gap: 40px;
			grid-template-columns: repeat(2, 1fr);
			grid-template-rows: repeat(2, 1fr);
			& > div {
				height: 80px;
				aspect-ratio: 1;
				background-color: var(--white);
				&:before {
					content: '';
					position: absolute;
					height: 20px;
					width: 80px;
					background-color: var(--black);
					translate: 0px -20px;
				}
			}
			& > div:nth-child(2) {
				transform: rotate(90deg);
			}

			& > div:nth-child(3) {
				transform: rotate(270deg);
			}
            &>div:nth-child(4){
                transform: rotate(180deg);
            }
		}
	}
</style>
