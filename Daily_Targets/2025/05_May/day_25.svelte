<div class="main">
	<div class="greenEye"></div>
	<div class="eye"></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--blue: #243d83;
		--green: #4a9a86;
		--yellow: #e3cc9e;
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
		overflow: hidden;
        background-color:var(--blue);
		& > .greenEye,
		& > .eye {
			position: absolute;
			height: 50px;
			width: 100px;
			background-color: var(--yellow);
			transform: translate(-130px);
			&:before,
			&:after {
				content: '';
				position: absolute;
				background-color: transparent;
				height: 165px;
				width: 160px;
				transform: translate(-30px, 10px);
				border-top-right-radius: 80px;
				border-top-left-radius: 80px;
				box-shadow: 0 0 0 50px var(--green);
			}
			&:after {
				transform: translate(-30px, -125px) rotate(-180deg);
			}
		}
		& > .eye {
			background-color: var(--yellow);
			transform: translate(130px);
			&:before,
			&:after {
				box-shadow: 0 0 0 50px var(--blue);
			}
		}
	}
</style>
