<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--red: #b53733;
		--black: #151109;
        background-color:var(--black);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		& > div {
			height: 200px;
			aspect-ratio: 1;
			background-color: var(--red);
			border-radius: 50%;
			clip-path: polygon(
				0 0,
				200px 0px,
				200px 151px,
				185px 151px,
				143px 109px,
				120px 131px,
                69px 80px,
                0px 149px,
				0 200px
			);
                &:before{
                position:absolute;
                content:'';
                height:20px;
                aspect-ratio:1;
                border-radius:50%;
                transform:translate(133px, 31px);
                background-color:var(--black);
            }
		}
	}
</style>

