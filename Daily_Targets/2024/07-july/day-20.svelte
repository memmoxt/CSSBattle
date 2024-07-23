<div class="main">
	<div class="center">
		<div></div>
		<div></div>
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
		box-sizing: content-box;
		--orange: #f48b26;
		--yellow: #feff58;
        background-color:var(--orange);
	}
	.main {
		height: 300px;
		width: 400px;
		display: grid;
		justify-content: center;
		align-items: center;
		& > .center {
			height: 200px;
			width: 280px;
			display: grid;
			gap: 20px;
			grid-template-columns: repeat(5, 40px);
			& > div {
				height: 200px;
				width: 40px;
				background-color: var(--yellow);
			}
			& > div:nth-last-child(1),
			div:nth-last-child(1):after {
				position: absolute;
				height: 280px;
                width:280px;
				border-radius:50%;
				transform: translate(-160px, -140px);
				background-color: var(--orange);
			}
			& > div:nth-last-child(1):after {
				content: '';
				transform: translate(320px, 0%);
			}
		}
	}
</style>

