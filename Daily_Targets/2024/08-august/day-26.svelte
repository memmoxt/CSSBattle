<div class="main">
	<div><div></div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--red: #b53733;
		--black: #000000;
		--white: #ffffff;
        background-color:var(--red);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		& > div {
			background-color: var(--black);
			height: 100px;
			width: 160px;
			border-radius: 30%/50%;
			position: absolute;
			& > div {
                position:absolute;
                height:100px;
                aspect-ratio:1;
                background-color:var(--white);
                border-radius:50%;
                transform:translate(30px, 30px);
                box-shadow: -0px -60px 0 0 var(--red);
			}
		}
	}
</style>

