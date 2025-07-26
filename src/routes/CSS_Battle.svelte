<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--white: #ffffff;
		--light: #9e8dec;
		--medium: #6855bf;
		--dark: #5528a5;
        background-color:var(--white);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		& > div {
			height: 50px;
			width: 200px;
			background-color: var(--light);
			border-radius: 10px/10px;
			translate: 0px -55px;
			&:before {
				content: '';
				position: absolute;
				height: 50px;
				width: 240px;
				background-color: var(--medium);
				translate: -20px 40px;
				border-radius: 10px/10px;
			}
            &:after{
				border-radius: 10px/10px;
                content:'';
                position: absolute;
                height: 110px;
                width: 280px;
                background-color: var(--light);
                translate: -40px 80px;
            }
		}
	}
</style>
