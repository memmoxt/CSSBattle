<div class="main">
	<div class="a"></div>
	<div class="i"></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--green: #668884;
		--white: #eed9d9;
        background-color: var(--green);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		position: absolute;
		& > .a {
			position: absolute;
			height: 240px;
			width: 150px;
			translate: -55px;
			background-color: var(--white);
			&:before {
				content: '';
				position: absolute;
				height: 60px;
				width: 70px;
				background-color: var(--green);
				translate: 40px 40px;
			}
			&:after {
				content: '';
				position: absolute;
				height: 100px;
				width: 70px;
				background-color: var(--green);
				translate: 40px 140px;
			}
		}
		& > .i {
            position:absolute;
			height: 40px;
			width: 70px;
			background-color: var(--white);
            translate: 110px -100px;
            &:before{
                content:'';
                position:absolute;
                height: 200px;
                width:40px;
                background-color: var(--white);
                translate: 15px 40px;
            }
		}
	}
</style>
