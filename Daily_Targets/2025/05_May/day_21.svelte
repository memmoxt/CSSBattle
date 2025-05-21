<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--red: #c53025;
		--yellow: #eddf5a;
        background-color:var(--yellow);
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
			height: 40px;
			width: 400px;
			background-color: var(--red);
			box-shadow:
				0 80px var(--red),
				0 -80px var(--red);
			&:before {
				content: '';
				position: absolute;
                height:200px;
                width:40px;
                background-color:var(--red);
                transform:translate(180px,-130px);
                box-shadow:-40px 0 var(--yellow), 40px 0 var(--yellow);

			}
		}
	}
</style>
