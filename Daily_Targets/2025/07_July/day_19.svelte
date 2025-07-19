<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--blue: #b6ebe7;
		--purple: #5e2bb7;
		--indigo: #9382e4;
        background-color:var(--blue);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		& > div {
			height: 160px;
			width: 80px;
			background-color: var(--blue);
			translate: 0 -0px;
			box-shadow: 0 0 0 40px var(--indigo);
			clip-path: polygon(-200px 0, 300px 0, 300px 200px, -200px 200px);
			&:before {
				content: '';
				position: absolute;
				height: 160px;
				width: 40px;
				background-color: var(--indigo);
				translate: -135px 0px;
				box-shadow: 310px 0 var(--indigo);
			}
			&:after {
				content: '';
				position: absolute;
				height: 80px;
				width: 135px;
				background-color: var(--purple);
				translate: -135px 40px;
                box-shadow: 215px 0 var(--purple);
			}
		}
	}
</style>
