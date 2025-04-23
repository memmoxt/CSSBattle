<div class="main">
	<div class="snowman">
        <div class="hat"></div>
        <div class="snow"></div>
        <div class="scarf"></div>
    </div>
</div>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: content-box;
        --red:#AC474B;
        --orange:#FFA63F;
        --white:#ffffff;
        --black:#0E1F2B;
        background-color: var(--red);
	}

	.main {
		height: 300px;
		width: 400px;
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
        &>.snowman{
            /* background-color: blue; */
            height:190px;
            width:100px;
            display:flex;
            justify-content: center;
            align-items: center;
            &>.hat{
                z-index:2;
            /* opacity: 0.5; */
                align-self: start;
                height:40px;
                aspect-ratio:1;
                background-color:var(--black);
                &:before{
                    content:'';
                    position:absolute;
                    height:10px;
                    width:40px;
                    transform:translateY(15px);
                    background-color:var(--white);
                }
                &:after{
                    content:'';
                    position:absolute;
                    height:5px;
                    width:60px;
                    background-color:var(--black);
                    transform:translate(-10px,40px);
                }
            }
            &>.snow{
                position:absolute;
                height:60px; 
                aspect-ratio:1;
                background-color:var(--white);
                transform:translateY(-25px);
                /* opacity:0; */
                border-radius:50%;
                z-index:0;
                box-shadow: 0px 70px 0px 20px var(--white);
                &:before{
                    content:'';
                    position:absolute;
                    height:10px;
                    aspect-ratio:1;
                    border-radius:50%;
                    background-color:var(--black);
                    transform: translate(15px, 18px);
                    box-shadow: 20px 0 var(--black);
                }
            }
            &>.scarf{
                position:absolute;
                height:18px;
                width:150px;
                transform:translateY(-2px);
                background-color:var(--red);
                &:before{
                    content:'';
                    position:absolute;
                    height:10px;
                    width:60px;
                    background-color:var(--orange);
                    transform:translate(45px, 4px);
                    border-radius:5px/5px;
                }
            }
        }
	}
</style>

