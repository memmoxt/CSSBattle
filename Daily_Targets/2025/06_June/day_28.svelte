<div class="main">
	<div></div>
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--white: #ffffff;
		--gray: #9cbbc2;
		--teal: #5a8d9a;
		--tealdark: #749faa;
		background-color: var(--white);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
		overflow: hidden;
		& > div:nth-child(1) {
			position: absolute;
			height: 140px;
			width: 340px;
			background-color: var(--gray);
			&:before {
				content: '';
				position: absolute;
				height: 310px;
				width: 80px;
				translate: 90px -90px;
				background-color: var(--gray);
				box-shadow: 80px 0 var(--tealdark);
			}
			&:after {
				content: '';
				position: absolute;
				height: 140px;
				width: 80px;
				translate: 90px 0;
				background-color: var(--tealdark);
				/* background-color:red; */
			}
		}
		& > div:nth-child(2) {
			height: 50px;
			width: 250px;
			background-color: var(--white);
			z-index: 2;
			&:before,&:after {
				content: '';
				position: absolute;
				height: 140px;
				width: 80px;
				/* background-color: var(--tealdark); */
				background-color: #5A8E9C;
				translate: 125px 50px;
				opacity: 1;
			}
            &:after{
				translate: 125px -140px;
            }
		}
	}
</style>
