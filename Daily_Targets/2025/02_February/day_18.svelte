<div class="main">
	<div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
		--green: #46ba67;
		--white: #d9d9d9;
		--black: #343d42;
        background-color:var(--green);
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
			position: absolute;
            bottom:0px;
			height: 200px;
            width:300px;
			background-color: var(--white);
            &:before{
                content:'';
                position:absolute;
                height:80px;
                aspect-ratio:1;
                background-color:var(--black);
                box-shadow:220px 0 var(--black);
            }
		}
	}
</style>

