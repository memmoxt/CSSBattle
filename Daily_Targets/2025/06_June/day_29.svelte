<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--black: #394257;
		--green: #48bf7d;
		--red: #d24444;
		--yellow: #fade8b;
		--white: #ffffff;
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
		overflow: hidden;
		& > div {
			height: 160px;
			width: 200px;
			background-color: var(--red);
			box-shadow:
				200px 0 var(--yellow),
				0px -160px var(--black),
				200px -160px var(--green);
			translate: -100px 80px;
			&:before {
				content: '';
				position: absolute;
				height: 80px;
				aspect-ratio: 1;
				border-radius: 50%;
				background-color: var(--white);
				translate: 30px -40px;
				box-shadow:
					130px 0 var(--white),
					260px 0 var(--white);
			}
            &::after{
                content:'';
                position:absolute;
                height:100px;
                aspect-ratio:1;
                background-color: var(--black);
                translate:20px -100px;
                box-shadow:260px 0 var(--green);
            }
		}
	}
</style>
