<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
        --green:#5A9F48;
        --white:#D9D9D9;
        --black:#000000;
        background-color:var(--green);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		& > div {
			height: 75px;
			width: 150px;
			box-shadow: 0 40px 0 60px var(--white);
			align-self: start;
			background-color: var(--green);
			&:before {
				content: '';
				position: absolute;
				height: 125px;
				width: 110px;
				translate: 20px 175px;
				box-shadow: 0 0 0 20px var(--green);
				background-color: var(--white);
			}
			&:after {
				content: '';
				position: absolute;
				height: 150px;
				aspect-ratio: 1;
				background-color: var(--white);
				border-radius: 50%;
				translate: 0 80px;
				box-shadow: 0 0 0px 60px var(--black);
				clip-path: polygon(-80px -80px, 220px -80px, 220px 75px, -80px 75px);
			}
		}
	}
</style>
