<div class="main">
	<div><div></div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--white: #ffffff;
		--black: #000000;
        background-color:var(--white);
	}
	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
        &>div{
            height:200px;
            width:300px;
            background-color:var(--black);
            transform:translate(0%,0%);
            display:flex;
            justify-content:center;
            align-items:center;
            & > div {
                background-color:var(--white);
                height: 200px;
                width: 100px;
                
                &:before {
                    content: '';
                    position: absolute;
                    height: 100px;
                    width: 200px;
                    background-color: var(--white);
                    transform: translate(-25%, 50%);
                }
            }
        }
	}
</style>

