<div class="main">
	<div></div>
</div>

<style>
* {
    margin: 0;
    padding: 0;
    box-sizing: content-box;
    --red: #d25b70;
    --white: #f7f3da;
    --yellow: #f6df96;
    --green: #6cb3a9;
}

.main {
    height: 300px;
    width: 400px;
    display: flex;
    justify-content: center;
    align-items: center;
    position: absolute;
    overflow: hidden;
    background-color:var(--red);

    &>div {
        position: absolute;
        height: 100px;
        aspect-ratio: 1;
        background-color: var(--white);
        /* opacity: 0.5; */
        bottom: 50px;

        &:before {
            content: '';
            position: absolute;
            height: 60px;
            aspect-ratio: 1;
            background-color:var(--green);
            transform-origin: 0px 0px;
            transform:rotate(217deg);
        }
        &:after{
            content:'';
            position:absolute;
            height:80px;
            aspect-ratio:1;
            background-color:var(--yellow);
            transform-origin:0 0;
            transform:translate(100px) rotate(-143deg);

        }
    }
}
</style>
