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
		--beige: #e8ad6d;
		--brown: #3b240c;
        background-color:var(--beige);
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
			height: 120px;
			width: 280px;
            position:absolute;
            overflow: hidden;
			& > div {
				height: 50px;
				width: 280px;
				background-color: var(--brown);
				&:before {
					content: '';
					position: absolute;
					height: 40px;
					border-radius: 50%;
					aspect-ratio: 1;
					background-color: var(--beige);
					translate: 30px 100px;
					box-shadow:
						0 0 0 30px var(--brown),
						180px 0 0 0 var(--beige),
						180px 0 0 30px var(--brown);
				}
				&:after {
					content: '';
					position: absolute;
					height: 50px;
					width: 60px;
					background-color: var(--brown);
                    translate: 110px 70px;
				}
			}
		}
	}
</style>
