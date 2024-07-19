<div class="main">
	<div class="bee">
		<div class="wing"></div>
		<div class="body">
			<div class="stripes"></div>
			<div class="eye"></div>
		</div>
	</div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--brown: #998235;
		--white: #ffffff;
		--yellow: #eff33c;
		--black: #191919;
		background: var(--brown);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
		& > .bee {
			height: 150px;
			aspect-ratio: 1;
			display: flex;
			justify-content: space-between;
			flex-wrap: wrap;
			align-content: space-between;
			& > .wing,
			& > .wing:before {
				height: 75px;
				aspect-ratio: 1;
				border-radius: 50% 50% 0 50%;
				background-color: var(--white);
			}
			& > .wing:before {
				content: '';
				position: absolute;
				transform: translate(75px, 0px) scaleX(-1);
				background-color: var(--white);
			}
			& > .body {
				position: absolute;
				width: 150px;
				height: 75px;
				background-color: var(--yellow);
				border-radius: 50px 50px 50px 50px;
				overflow: hidden;
				transform: translateY(75px);
				& > .stripes {
					position: absolute;
					height: 75px;
					width: 25px;
					background-color: var(--black);
					box-shadow:
						35px 0 var(--black),
						70px 0 var(--black);
				}
				& > .eye {
					position: absolute;
					height: 15px;
					aspect-ratio: 1;
					border-radius: 50%;
					background-color: var(--black);
					transform: translate(115px, 20px);
				}
			}
		}
	}
</style>
