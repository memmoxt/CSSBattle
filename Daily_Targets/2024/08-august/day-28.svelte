<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--red: #eb5868;
		--dark_red: #942f3a;
		--white: #eed9d9;
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		background-color: var(--white);
		& > div {
			background-color: green;
			position: absolute;
			top: 107px;
			height: 139px;
			width: 62px;
            /* opacity:50%; */
		}
		& > div:nth-child(1) {
			transform: translate(-50%, 0px);
			clip-path: polygon(61px 1px, 61px 139px, 31px 139px, 31px 74px, 0px 105px, 0px 62px);
			background-color:var(--red);
		}
		& > div:nth-child(2) {
			transform: translate(48%, 0px);
			clip-path: polygon(0 0.90px, 62px 62px, 62px 105px, 30px 74px, 30px 139px, 0px 139px);
			background-color: var(--dark_red);
		}
	}
</style>

