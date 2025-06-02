<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--green: #23384b;
		--white: #d9d9d9;
		--red: #d36354;
        background-color:var(--green);
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
			height: 60px;
			aspect-ratio: 1;
			background-color: var(--green);
			border-radius: 50%;
			box-shadow:
				0 0 0 20px var(--red),
				0 0 0 40px var(--white);
			&:before {
                content:'';
                position:absolute;
                height:100px;
                width:30px;
                transform:translate(15px,10px);
                background-color:var(--green);
			}
		}
	}
</style>
