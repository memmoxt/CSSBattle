<div class="main">
	<div>
		<div></div>
	</div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--green: #62e383;
		--brown: #3b240c;
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
			height: 180px;
			width: 200px;
			overflow: hidden;
			&:before {
				content: '';
				position: absolute;
				height: 180px;
				aspect-ratio: 1;
				background-color: var(--brown);
				border-radius: 50%;
				translate: 10px 0px;
				box-shadow:
					-70px 0 var(--brown),
					70px 0 var(--brown);
			}
			& > div {
				position: absolute;
                height: 10px;
                width:80px;
                background-color:var(--green);
                translate:60px 100px;
                &:before{
                    position:absolute;
                    content:'';
                    height: 20px;
                    aspect-ratio:1;
                    background-color:var(--green);
                    border-radius:50%;
                    translate: 0px -40px;
                    box-shadow: 60px 0 var(--green);
                }
			}
		}
	}
</style>
