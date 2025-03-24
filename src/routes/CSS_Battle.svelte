<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--red: #e3516e;
		--darkred: #66284a;
        background-color:var(--red);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		flex-wrap: wrap;
		position: absolute;
		overflow: hidden;
		& > div {
			height: 80px;
			aspect-ratio: 1/1;
			position: absolute;
			background-color: var(--darkred);
			transform: translate(-130px, -80px);
			box-shadow:
				260px 0 var(--darkred),
				260px 160px var(--darkred),
				0px 160px var(--darkred);
			&:before {
				content: '';
				position: absolute;
				height: 20px;
				width: 340px;
				box-shadow:
					0 40px var(--darkred),
					0 180px var(--darkred),
					0 220px var(--darkred);
				background-color: var(--darkred);
			}
			&:after {
				content: '';
				position: absolute;
				width: 20px;
				height: 240px;
				background-color: var(--darkred);
				box-shadow:
					40px 0 var(--darkred),
					280px 0 var(--darkred),
					320px 0 var(--darkred);
			}
		}
	}
</style>
