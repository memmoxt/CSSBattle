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
		--red: #84271c;
		--black: #191210;
        background-color:var(--black);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		& > div:nth-child(1) {
			height: 150px;
			width: 250px;
			border-radius: 25px/25px;
			background-color: var(--black);
			z-index: 2;
		}
		& > div:nth-child(2),
		div:nth-child(2):before,
		div:nth-child(3),
		div:nth-child(3):before {
			position: absolute;
			height: 75px;
			width: 240px;
			background-color: var(--red);
			border-top-left-radius: 38px;
			border-bottom-left-radius: 38px;
			right: 0;
			top: 0;
		}
		& > div:nth-child(2):before,
		div:nth-child(3):before {
			content: '';
			width: 75px;
			height: 200px;
			border-bottom-right-radius: 38px;
		}
		& > div:nth-child(2):after,
		div:nth-child(3):after {
			content: '';
			width: 100px;
			height: 100px;
			background-color: var(--red);
			position: absolute;
			right: 0;
		}
        &>div:nth-child(3){
            left:0;
            top:75%;
            transform:scale(-1);

        }
	}
</style>

