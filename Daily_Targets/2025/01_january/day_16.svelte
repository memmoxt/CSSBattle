<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		position: absolute;
		flex-wrap: wrap;
		gap: 20px;
		--blue: #a1e6e4;
		--purple: #8f77da;
        background-color:var(--purple);
		& > div {
            position:absolute;
			height: 332px;
			width: 70px;
            top:-76px;
			background-color: var(--blue);
            transform:rotate(-35deg);
		}
        &>div:nth-child(2){
            transform:rotate(35deg);
        }
	}
</style>

