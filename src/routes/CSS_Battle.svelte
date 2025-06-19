<div class="main">
	<div class="border">
		<div></div>
	</div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--white: #fefeff;
		--blue: #5aa4b7;
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
		overflow: hidden;
	}
	.border {
		height: 260px;
		width: 360px;
		background-color: var(--white);
		box-shadow: 0 0 0 20px var(--blue);
		opacity: 0.5;
		& > div {
			height: 100px;
			aspect-ratio: 1;
			background-color: var(--blue);
			border-radius: 50%;
			transform: translate(50px, 80px);
			box-shadow: 160px 0 var(--blue);
			&::before {
				content: '';
				position: absolute;
                height:40px;
                width:200px;
                transform:translate(30px, 30px);
                border-radius: 20px/20px;
                background-color:var(--white);
			}
            &::after{
                content:'';
                position:absolute;
                height:20px;
                width:40px;
                background-color:var(--blue);
                transform:translate(50px,40px);
                box-shadow: 60px 0 var(--blue) , 120px 0 var(--blue);
            }

		}
	}
</style>
