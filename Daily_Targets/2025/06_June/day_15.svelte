<div class="main">
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

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--green: #97ae41;
		--blue: #334f9f;
	}
	.main {
		height: 300px;
		width: 400px;
		display: grid;

		justify-content: center;
		align-items: center;
		position: absolute;
		overflow: hidden;
		grid-template-columns: 40px 1fr 40px;
		grid-template-rows: 90px repeat(3, 1fr) 90px;
		& > div {
			position: relative;
			height: 100%;
			width: 100%;
		}
		& > div:nth-child(odd) {
			background-color: var(--blue);
		}
		& > div:nth-child(even) {
			background-color: var(--green);
		}
	}
</style>
