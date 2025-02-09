<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--blue: #6592cf;
		--darkblue: #243d83;
        background-color:var(--blue);
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
			height: 270px;
			width: 150px;
			background-color: var(--darkblue);
			&:before {
				content: '';
				position: absolute;
				height: 150px;
				width: 320px;
				background-color: var(--darkblue);
				top: 75px;
				left: 40px;
			}
            &:after{
                content:'';
                position:absolute;
                background-color:var(--darkblue);
                height:50px;
                border-radius:50%;
                aspect-ratio:1;
                top:125px;
                left:175px;
                box-shadow:0 0 0 95px var(--blue);
            }
		}
	}
</style>

