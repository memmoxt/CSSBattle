<div class="main">
	<div>
		<div></div>
		<div></div>
		<div></div>
		<div></div>
	</div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--black: #282828;
		--white: #f9ddc6;
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
		overflow: hidden;
        background-color:var(--black);
		& > div {
			position: absolute;
			height: 240px;
			aspect-ratio: 1;
			background-color: var(--black);
			display: flex;
			justify-content: space-between;
			align-items: space-between;
			flex-wrap: wrap;
            gap:80px;
			& > div {
				height: 80px;
				aspect-ratio: 1;
				background-color: var(--white);
				&:before {
					content: '';
					position: absolute;
					height: 40px;
					aspect-ratio: 1;
					background-color: var(--black);
				}
			}
			& > div:nth-child(2) {
				transform: rotate(90deg);
			}
			& > div:nth-child(3) {
				transform: rotate(-90deg);
			}
            &>div:nth-child(4){
                transform:rotate(180deg);
            }
		}
	}
</style>
