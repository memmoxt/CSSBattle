<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--blue: #328fc1;
		--darkblue: #050044;
        background-color:var(--darkblue);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		& > div {
			height: 60px;
			aspect-ratio: 1;
			background-color: var(--darkblue);
			border-radius: 50%;
            transform:translateY(-60px);
            box-shadow:0 0 0px 10px var(--blue),
                0 40px 0 0px var(--blue),
                0 70px 0 0px var(--darkblue),
                0 70px 0 10px var(--blue),
                0 110px 0 0 var(--blue),
                0 140px 0 0 var(--darkblue),
                0 140px 0 10px var(--blue);
		}
	}
</style>

