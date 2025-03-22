<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--yellow: #fade8b;
		--red: #e3516e;
        background-color:var(--yellow);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		flex-wrap: wrap;
		position: absolute;
		overflow: hidden;
		& > div {
			position: absolute;
			height: 140px;
			width: 250px;
			background-color: var(--red);
			/* opacity: 0.5; */
			clip-path: polygon(
				0px 50px,
				62px 0px,
				188px 0px,
				100% 50px,
				100% 90px,
				188px 100%,
				62px 100%,
				0px 90px
			);
			&:before {
				content: '';
				position: absolute;
				height: 40px;
				width: 100%;
				background-color: var(--yellow);
				top: 50px;
			}
			&:after {
				content: '';
				position: absolute;
				height: 40px;
				aspect-ratio: 1;
				top: 50px;
				left: 105px;
				border-radius: 50%;
				box-shadow: 0 0 0 30px var(--yellow);
				background-color: var(--red);
			}
		}
	}
</style>

