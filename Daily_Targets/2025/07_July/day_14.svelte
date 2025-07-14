<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--white: #ceedff;
		--dark: #05476c;
		--blue: #2bbbf3;
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
			width: 350px;
			aspect-ratio: 1;
			border-radius: 50%;
			background-color: var(--blue);
			translate: 0px -40px;
			clip-path: polygon(-150px 0, 400px 0px, 400px 255px, 0px 255px);
			&:before {
				content: '';
				position: absolute;
				height: 300px;
				aspect-ratio: 1;
				background-color: var(--white);
				border-radius: 50%;
				translate: 25px -60px;
			}
            &:after{
                content:'';
                position:absolute;
                height:160px;
                width:350px;
                background-color:var(--dark);
                translate: 0px 175px;
            }
		}
	}
</style>
