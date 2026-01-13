<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--lightgreen: #45b45b;
		--darkgreen: #194247;
        background-color: var(--lightgreen);
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
			height: 50px;
			aspect-ratio: 1;
			background-color: var(--darkgreen);
			translate: 0px -95px;
			border-radius: 50%;
			&:before,&:after {
				content: '';
				position: absolute;
				height: 50px;
				aspect-ratio: 1;
				background-color: var(--darkgreen);
				translate: -155px;
				box-shadow:
					0px 190px var(--darkgreen),
					310px 0px var(--darkgreen),
					310px 190px var(--darkgreen);
			}
            &:after{
                height: 120px;
                width: 50px;
                background-color: var(--darkgreen);
                translate: -155px 60px;
                box-shadow: 310px 0px var(--darkgreen);
            }
            
		}
	}
</style>
