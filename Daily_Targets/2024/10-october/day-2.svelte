<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--blue: #6b7cbe;
		--green: #abc497;
		--white: #fffefe;
        background-color:var(--blue);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		flex-wrap: wrap-reverse;
		flex-direction: column;
		overflow: hidden;
		& > div:nth-child(1) {
			top: 134px;
			position: absolute;
			height: 600px;
			aspect-ratio: 1;
			background-color: var(--white);
			border-radius: 50%;
			clip-path: polygon(326px 0px, 350px 166px, 250px 166px, 273px 0px);
            z-index:1;
		}
		& > div:nth-child(2) {
			top: 134px;
			position: absolute;
			height: 600px;
			aspect-ratio: 1;
			background-color: var(--green);
			border-radius: 50%;
            z-index:0;
		}
	}
</style>

