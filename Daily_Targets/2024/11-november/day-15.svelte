<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--orange: #ea9a52;
		--wine: #a82973;
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
        background-color:var(--orange);

		& > div {
            top:54px;
            position:absolute;
			height: 56px;
            border-radius:50%;
			aspect-ratio: 1;
            background-color:var(--wine);
            &:before{
                position:absolute;
                content:'';
                height:120px;
                width:56px;
                background-color:var(--wine);
                top:72px;
            }
		}
	}
</style>

