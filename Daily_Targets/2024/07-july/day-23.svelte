<div class="main">
	<div class="waves">
		<div></div>
	</div>
	<div class="waves">
        <div></div>
    </div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--blue: #4f77ff;
		--white: #eff8fe;
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: start;
        background-color:var(--white);
		& > .waves {
			height: 125px;
			width: 400px;
			background-color: var(--blue);
			overflow: hidden;
			& > div {
				height: 150px;
				aspect-ratio: 1;
				background-color: var(--white);
				border-radius: 50%;
				transform: translateY(-75px);
				box-shadow:
					125px 0 0 var(--white),
					250px 0 0 var(--white);
			}
		}
		& > .waves:nth-child(2) {
            position:absolute;
			align-self: end;
            transform:scaleY(-1);
		}
	}
</style>
