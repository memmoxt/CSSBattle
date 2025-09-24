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
		--blue: #7dddeb;
		--purple: #9a5dcb;
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
			position: absolute;
			height: 160px;
			aspect-ratio: 1;
			display: grid;
			grid-template-columns: repeat(2, 1fr);
			grid-template-rows: repeat(2, 1fr);
			gap: 20px;
			& > div {
				position: relative;
				height: 70px;
				aspect-ratio: 1;
				&:before {
					content: '';
					position: absolute;
					height: 30px;
					background-color: var(--purple);
					aspect-ratio: 1;
					box-shadow: 40px 0 var(--purple);
				}
				&:after {
					content: '';
					position: absolute;
					height: 30px;
					width: 70px;
					background-color: var(--purple);
					translate: 0 40px;
				}
			}
			& > div:nth-child(2) {
				transform: rotate(-90deg);
			}
			& > div:nth-child(3) {
				transform: rotate(90deg);
			}
			& > div:nth-child(4) {
				transform: rotate(180deg);
			}
		}
	}
</style>
