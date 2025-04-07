<div class="main">
	<div></div>
</div>

<style>
* {
    margin: 0;
    padding: 0;
    box-sizing: content-box;
    --black: #191919;
    --purple: #714B67;
    --grey: #8F8F8F;
}

.main {
    height: 300px;
    width: 400px;
    display: flex;
    justify-content: center;
    align-items: center;
    position: absolute;
    overflow: hidden;
    background-color:var(--black);

    &>div {
        height: 40px;
        aspect-ratio: 1;
        border-radius: 50%;
        transform: translate(-123px, 12px);
        background-color: var(--black);
        /* opacity: 0.5; */
        box-shadow: 0 0 0 20px var(--purple), 
            82px 0 var(--black), 
            82px 0 0 20px var(--grey),
            164px 0 var(--black),
            164px 0 0 20px var(--grey),
            246px 0 var(--black),
            246px 0 0 20px var(--grey);
            &:before{
            position:absolute;
            content:'';
            transform:translate(122px, -40px);
            border-radius:20px/20px;
            height:70px;
            width:20px;
            background-color:var(--grey);
        }
    }
}
</style>
