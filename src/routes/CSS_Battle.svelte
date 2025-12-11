<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--white: #f7e5fb;
		--purple: #62306d;
        background-color: var(--white);
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
			height: 100px;
			aspect-ratio: 1;
			background-color: var(--white);
			border-radius: 50%;
			box-shadow: 0 0 0 30px var(--purple);
			&:before {
				content: '';
				position: absolute;
				height: 30px;
				width: 60px;
				background-color: var(--purple);
				transform: translate(87px, 97px) rotate(45deg);
				border-radius: 50px;
			}
		}
	}
</style>
