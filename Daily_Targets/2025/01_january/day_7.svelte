<div class="main">
	<div></div>
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
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
		--green: #4a9a86;
		--black: #4c4c6b;
		--yellow: #fae29e;
        background-color:var(--green);
		& > div {
			height: 80px;
			aspect-ratio: 1;
			background-color: var(--black);
			&:before {
				content: '';
				position: absolute;
				height: 40px;
				aspect-ratio: 1;
				background-color: var(--yellow);
				border-radius: 50%;
				transform: translate(20px, 20px);
			}
		}
        &>div:nth-child(2){
            background-color:var(--yellow);
            &:before{
                background-color:var(--black);
            }
        }
	}
</style>

