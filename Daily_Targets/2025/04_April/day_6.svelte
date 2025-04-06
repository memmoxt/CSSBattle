<div class="main">
	<div class=""></div>
	<div class=""></div>
</div>

<style>
* {
    margin: 0;
    padding: 0;
    box-sizing: content-box;
    --purple: #2a2753;
    --yellow: #c3c441;
    --red: #e25c57;
}

.main {
    height: 300px;
    width: 400px;
    display: flex;
    justify-content: center;
    align-items: center;
    position: absolute;
    overflow: hidden;
    background-color:var(--purple);

    &>div {
        position: relative;
        height: 200px;
        width: 200px;
        /* opacity: 0.5; */
        clip-path: polygon(0px 95px, 100px 5px, 200px 95px, 200px 200px, 0px 200px)
    }

    &>div:nth-child(1) {
        align-self: end;
        transform: translate(200px);
        background-color: var(--red);
    }

    &>div:nth-child(2) {
        align-self: end;
        transform: rotate(180deg) translate(200px, 100px);
        background-color: var(--yellow);
    }
}
</style>

