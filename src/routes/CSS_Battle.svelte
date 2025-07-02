<div class="main">
	<div>
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
		--blue: #4f77ff;
		--white: #eff8fe;
        background-color:var(--white)
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		& > div {
            margin-top:10px;
            margin-right:10px;
			height: 210px;
			width: 310px;
			display: flex;
			gap: 0px 60px;
			justify-content: end;
			align-items: start;
			background-color: var(--blue);
			/* opacity: 0.5; */
			&:before,
			&:after {
				content: '';
				position: absolute;
				height: 100px;
				width: 60px;
				background-color: var(--white);
				translate: -30px 0px;
			}
			&:after {
				translate: -210px -0px;
				height: 60px;
				width: 60px;
			}
			& > div {
				height: 200px;
				width: 30px;
				background-color: var(--white);
			}
		}
	}
</style>
