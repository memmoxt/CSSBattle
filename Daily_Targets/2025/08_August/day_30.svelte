<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--green: #a1e8a7;
		--red: #d2495c;
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
			position: absolute;
			height: 250px;
			width: 250px;
			background-color: var(--red);
			translate: 0px 25px;
			&:before {
				content: '';
				position: absolute;
				height: 50px;
				width: 150px;
				background-color: var(--green);
				translate: 50px 50px;
				box-shadow: 0px 100px var(--green);
			}
			&:after {
				content: '';
				position: absolute;
				height: 150px;
				width: 50px;
				background-color: var(--green);
				translate: 100px 100px;
			}
		}
	}
</style>
