<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--lightblue: #7dddeb;
		--darkblue: #2a4cac;
        background-color: var(--lightblue);
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
			height: 60px;
			width: 340px;
			translate: 0px -30px;
			background-color: var(--darkblue);
			&:before {
				content: '';
				position: absolute;
				height: 30px;
				aspect-ratio: 1;
				background-color: var(--darkblue);
				translate: 0 -50px;
				box-shadow: 310px 0px var(--darkblue);
			}
			&:after {
				content: '';
				position: absolute;
				height: 90px;
				width: 30px;
				background-color: var(--darkblue);
				translate: 0 80px;
				box-shadow: 310px 0 var(--darkblue);
			}
		}
	}
</style>
