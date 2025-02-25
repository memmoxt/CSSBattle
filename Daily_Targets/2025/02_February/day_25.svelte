<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--yellow: #f2eaa8;
		--blue: #3f4869;
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
            position:absolute;
            top:0px;
            height:50px;
            width:360px;
            background-color:var(--blue);
            box-shadow:0 250px var(--blue);
			&:before {
				content: '';
				position: absolute;
				height: 100px;
				width: 130px;
				top: 100px;
				left: 115px;
				background-color: var(--yellow);
				box-shadow: 0 0 0 25px var(--blue);
			}
			&:after {
                content:'';
				position: absolute;
                top:125px;
                left:135px;
				height: 50px;
				width: 90px;
				background-color: var(--blue);
			}
		}
	}
</style>

