
<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--white: #fefaed;
		--beige: #f9d9bf;
		--brown: #d4a29f;
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
        background-color:var(--white);
        &>div{
            height:180px;
            width:240px;
            background-color:var(--beige);
            /* opacity:0.5; */
            &:before{
                content:'';
                position:absolute;
                height:90px;
                width:60px;
                background-color:var(--brown);
                box-shadow:180px 90px var(--brown);
            }

        }
	}
</style>
