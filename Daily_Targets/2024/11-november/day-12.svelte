<div class="main">
	<div>
		<div></div>
	</div>
	<div>
		<div></div>
	</div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--red: #e05947;
		--white: #f0f0f0;
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		& > div:nth-child(1),
		& > div:nth-child(2) {
            position:absolute;
			align-self: flex-start;
			height: 50%;
			width: 100%;
			background-color: var(--red);
			display: flex;
			justify-content: center;
			overflow: hidden;
			& > div {
				height: 85px;
				width: 360px;
				background-color: var(--white);
				box-shadow: 0 140px 0 0 var(--white);
				&:before {
					content: '';
					position: absolute;
					height: 20px;
					width: 130px;
					background-color: var(--red);
					transform: translate(115px, 65px);
				}
			}
		}
        &> div:nth-child(2){
            transform:scaleY(-1);
            align-self:end;
        }
	}
</style>

