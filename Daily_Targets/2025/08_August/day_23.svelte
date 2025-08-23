<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--yellow: #fade8b;
		--red: #d2495c;
		--pink: #f28997;
        background-color:var(--yellow);
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
            position:absolute;
            height: 100px;
            aspect-ratio:1;
            border-radius:50%;
            background-color:var(--red);
            translate:-50px -30px;
            box-shadow: 100px 0 var(--red);
			&:before {
				content: '';
				position: absolute;
				height: 200px;
				aspect-ratio: 1;
				background-color: var(--red);
				border-radius: 50%;
				translate: -0px -40px;
				clip-path: polygon(0 85px, 200px 85px, 200px 200px, 0px 200px);
			}
            &:after{
                content:'';
                position:absolute;
                height: 18px;
                aspect-ratio:1;
                border-radius:50%;
                background-color: var(--pink);
                translate: 175px 35px; 
                box-shadow: -21px -21px 0 4px var(--pink);
            }

		}
	}
</style>
