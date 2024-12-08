<div class="main">
	<div></div>
    <div></div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		--white: #dbd7f6;
		--purple: #6255aa;
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
			position: absolute;
			top: 0px;
			height: 150px;
			width: 400px;
			background-color: var(--purple);
			&:before,
			&:after {
				position: absolute;
				content: '';
			}
			&:before {
				top: 50px;
				left: 75px;
				height: 100px;
				width: 250px;
				background-color:  var(--white);
			}
			&:after {
				top: 100px;
				left: 150px;
				height: 50px;
				width: 100px;
				background-color: var(--purple);
			}
		}
        &>div:nth-child(2){
            top:150px;
            transform:scale(-1);
            background-color:var(--white);
            &:before{
                background-color:var(--purple);
            }
            &:after{
                background-color:var(--white);
            }
        }

	}
</style>

