
<div class="main">
	<div>
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

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--pink: #f7bed9;
		--fuchsia: #f069ab;
		--rose: #ec0076;
		background-color: var(--pink);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		background-color: var(--green);
		& > div {
			height: 100px;
			width: 340px;
			display: grid;
			gap: 20px;
			grid-template-columns: 1fr 100px 1fr 100px;
			grid-template-rows: 1fr 1fr;
			& > div {
				height: 100%;
				width: 100%;
				border-radius: 50px/50px;
			}
			& > div:nth-child(2n + 1) {
				background-color: var(--fuchsia);
			}
			& > div:nth-child(2n) {
				background-color: var(--rose);
			}
		}
	}
</style>
