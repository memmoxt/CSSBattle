<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		/* box-sizing: content-box; */
		box-sizing: border-box;
		--blue: #328fc1;
		--darkblue: #243d83;
		--yellow: #ebe77e;
        background-color:var(--blue);
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
			height: 220px;
			aspect-ratio: 1;
			background-color: var(--darkblue);
			clip-path: polygon(
				0 0,
				30px 0px,
				30px 57px,
				163px 190px,
				220px 190px,
				220px 220px,
				0px 220px
			);
			&:before {
				content: '';
				position: absolute;
                height:90px;
                aspect-ratio:1;
                background-color: var(--yellow);
                translate:30px 100px;
                clip-path: polygon(0 0, 100% 100%, 0 100%);
			}
		}
	}
</style>
