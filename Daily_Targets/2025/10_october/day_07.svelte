<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--blue: #050044;
		--red: #d62e65;
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
		& > div:nth-child(1) {
			position: absolute;
			height: 158px;
			width: 100%;
			translate: 0 17px;
			background-color: green;
			overflow: hidden;
			&:before {
				content: '';
				position: absolute;
				height: 136px;
				aspect-ratio: 1;
				translate: 0px -8px;
				background-color: var(--blue);
				box-shadow:
					264px 0 var(--blue),
					0 0 0 300px var(--red);
			}
			&:after {
				content: '';
				position: absolute;
				height: 160px;
				aspect-ratio: 1;
				background-color: var(--red);
				border-radius: 50%;
				translate: 56px 48px;
				box-shadow: 128px 0 var(--red);
			}
		}
        &>div:nth-child(2){
            position:absolute;
            height:128px;
            width: 68px;
            translate: 0 32px;
            background-color: var(--blue);
        }
	}
</style>
