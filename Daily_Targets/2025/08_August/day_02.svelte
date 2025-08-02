<div class="main">
	<div>
		<div>
			<div></div>
			<div></div>
			<div></div>
			<div></div>
			<div></div>
			<div></div>
			<div></div>
			<div></div>
			<div></div>
			<div></div>
			<div></div>
			<div></div>
		</div>
	</div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		/* box-sizing: content-box; */
		box-sizing: border-box;
		--green: #31938c;
		--white: #ffffff;
        background-color:var(--green);
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
			height: 250px;
			width: 280px;
			background-color: var(--white);
			border-radius: 20px/20px;
			display: flex;
			justify-content: center;
			align-items: center;
			& > div {
				display: grid;
				justify-items: center;
				align-items: center;
				height: 160px;
				width: 220px;
				background-color: var(--green);
				translate: 0px 15px;
				grid-template-rows: repeat(3, 1fr);
				grid-template-columns: repeat(4, 1fr);
				gap: 0px 0px;
				padding: 5px 10px;
				& > div {
					height: 30px;
					aspect-ratio: 1;
					background-color: var(--white);
				}
				& > div:nth-child(1),
				div:nth-child(12) {
					background-color: var(--green);
				}
			}
		}
	}
</style>
