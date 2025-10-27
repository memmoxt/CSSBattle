<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--white: #fffce2;
		--beige: #c1a162;
		--brown: #7c3219;

	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		overflow: hidden;
		position: absolute;
        background-color: var(--white);
		& > div {
            position:absolute;
            height: 220px;
            width:300px;
            background-color: var(--white);
            overflow: hidden;
			&:before {
                content:'';
				position: absolute;
				height: 140px;
				aspect-ratio: 1;
				background-color: var(--beige);
				border-radius: 50%;
				translate: 80px 80px;
				box-shadow: 0 0 0 80px var(--brown);
			}
            &:after{
                content:'';
                position:absolute;
                width:300px;
                height: 80px;
                background-color: var(--beige);
                translate:0px 150px;
            }
		}
	}
</style>
