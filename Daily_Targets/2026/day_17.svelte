<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--blue: #4fa9c0;
		--yellow: #f4da64;
		--purple: #2b2a4a;
        background-color: var(--blue);
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
			height: 160px;
			width: 160px;
			translate: 30px;
			background-color: var(--yellow);
			&:before {
				content: '';
				position: absolute;
				height: 80px;
				width: 280px;
				background-color: var(--yellow);
				translate: -90px 80px;
			}
            &:after{
                content:'';
                position:absolute;
                height: 60px;
                aspect-ratio:1;
                background-color: var(--purple);
                border-radius: 50%;
                translate: -60px 130px;
                box-shadow: 160px 0 var(--purple);
            }
		}
	}
</style>
