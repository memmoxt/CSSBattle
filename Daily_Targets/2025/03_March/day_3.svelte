<div class="main">
	<div><div></div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--yellow: #eac049;
		--grey: #343d42;
        background-color:var(--yellow);
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
			transform: translate(-80px, -80px);
			&:before {
				content: '';
				position: absolute;
				height: 160px;
				aspect-ratio: 1;
				background-color: var(--grey);
				/* opacity: 0.5; */
				border-radius: 50%;
				clip-path: polygon(0 0, 160px 0px, 160px 80px, 0 80px);
			}
			& > div {
				position: absolute;
				height: 80px;
				aspect-ratio: 1;
				background-color: var(--grey);
				border-radius: 50%;
				transform: translateY(40px);
				/* opacity: 0.5; */
				&:before {
					position: absolute;
					content: '';
					height: 80px;
					aspect-ratio: 1;
					border-radius: 50%;
					background-color: var(--yellow);
					transform: translate(80px);
				}
				&:after {
					position: absolute;
					content: '';
					height: 40px;
					aspect-ratio: 1;
					background-color: var(--yellow);
					border-radius: 50%;
					transform: translate(20px, 60px);
				}
			}
		}
	}
</style>

