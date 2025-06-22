<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--green: #48bf7d;
		--grey: #394257;
		background-color: var(--green);
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
			height: 70px;
			aspect-ratio: 1;
			background-color: var(--grey);
			transform: rotate(-45deg);
			/* opacity: 0.5; */
			&:before {
				content: '';
				position: absolute;
				height: 72px;
				aspect-ratio: 1;
				background-color: var(--green);
				transform: translate(35px, 35px) rotate(90deg);
				border-radius: 10px/10px;
			}
			&:after {
				content: '';
				position: absolute;
				border-top: 50px solid var(--green);
				border-right: 0px solid var(--green);
				border-bottom: 50px solid var(--green);
				border-left: 50px solid var(--grey);
				transform: rotate(45deg) translate(47px, -18px);
			}
		}
	}
</style>
