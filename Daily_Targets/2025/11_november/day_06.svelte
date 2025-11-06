<div class="main">
	<div>
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
		--yellow: #ebcb58;
		--zinc: #556d7f;
        background-color: var(--zinc);
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
			height: 230px;
			width: 320px;
			display: grid;
			grid-template-rows: 1fr;
			grid-template-columns: repeat(3, 1fr);
			gap: 10px;

			& > div {
				content: '';
				position: relative;
				height: 100px;
				aspect-ratio: 1;
				border-radius: 50%;
				background-color: var(--yellow);
				&:before {
					content: '';
					position: absolute;
					height: 150px;
					width: 100px;
					translate: 0px 80px;
					background-color: var(--yellow);
				}
			}
			& > div:nth-child(2) {
				transform: scale(-1);
				align-self: end;
			}
		}
	}
</style>
