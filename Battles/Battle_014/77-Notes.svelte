<div class="main">
	<div class="music">
		<div class="crotchet"></div>
		<div class="crotchet"></div>
		<div class="crotchet"></div>
		<div class="crotchet"></div>
	</div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--black: #191919;
		--red: #fe5f55;
		--red2: #a64942;
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
        background:var(--black);
		& > .music {
			height: 120px;
			width: 290px;
			display: grid;
			gap: 0px 20px;
			grid-template-columns: repeat(4, 50px);
			& > .crotchet {
				height: 40px;
				width: 50px;
				border-radius: 40px/30px;
				align-self: end;
				background-color: var(--red);
				&:before {
					content: '';
					position: absolute;
					height: 100px;
					width: 10px;
					transform: translate(40px, -80px);
					background-color: var(--red);
				}
			}
			& > div:nth-child(1) {
				&:after {
					content: '';
					position: absolute;
					width: 70px;
					height: 10px;
					transform: translate(50px, -80px);
					background-color: var(--red);
				}
			}
			& > div:nth-child(3) {
					background-color: var(--red2);
                &:before{
					background-color: var(--red2);
                }
				&:after {
					content: '';
					position: absolute;
					width: 30px;
					height: 10px;
					transform: translate(50px, -80px);
					background-color: var(--red2);
				}
			}
			& > div:nth-child(4) {
				&:after {
					content: '';
					position: absolute;
					width: 30px;
					height: 10px;
					transform: translate(50px, -80px);
					background-color: var(--red);
					box-shadow: 0 20px var(--red);
				}
			}
		}
	}
</style>


