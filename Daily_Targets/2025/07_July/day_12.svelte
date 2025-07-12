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
		--purple: #504b72;
		--yellow: #fffbcc;
        background-color:var(--purple);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		--column: 20px;

		& > div {
			height: 220px;
			width: 320px;
			display: grid;
			grid-template-rows: 1fr var(--column) 1fr var(--column) 1fr;
			grid-template-columns: 1fr 120px 1fr;
			& > div:nth-child(2n + 1) {
				background-color: var(--yellow);
			}
			& > div{
				background-color: var(--purple);
			}
		}
	}
</style>
