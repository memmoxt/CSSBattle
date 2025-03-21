<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--light: #a9fffc;
		--green: #1a353c;
		--gray: #31798f;
        background-color:var(--light);
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
			border-top: 0px solid transparent;
			border-right: 150px solid transparent;
			border-bottom: 120px solid var(--green);
			border-left: 150px solid transparent;
			position: absolute;
			top: 60px;
			height: 0px;
			width: 0px;
			&:before {
				content: '';
				position: absolute;
				background-color: var(--gray);
				height: 120px;
				width: 40px;
				transform: translate(-120px, 120px);
				box-shadow:
					100px 0 0 0 var(--gray),
					200px 0 0 0 var(--gray);
			}
		}
	}
</style>

