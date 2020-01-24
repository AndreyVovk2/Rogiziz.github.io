<template>

    <div class="main-content">
        <header>
            <section class="headers">
                <div class="header">
                    <div class="title"><b>Logo Logo</b></div>
                    <nav>
                        <div class="list">

                            <div class="hamburger">
                                <img src="../assets/Rectangle.png" alt="">
                                <img src="../assets/Rectangle.png" alt=""></div>
                            <ul class="menu">
                                <li>Commercial</li>
                                <li>Editorial</li>
                                <li>Reportage</li>
                                <li>Meet Me</li>
                            </ul>
                        </div>
                    </nav>
                </div>
            </section>
        </header>
        <main>
            <section class="main-content">
                <div>
                    <span class="drag-me">Drag me</span>
                    <div class="body-image">
                        <div class="main-image-container">
                            <img class="main-image" src="../assets/image1.png" alt="image">
                            <img class="two-image" src="../assets/image2.png" alt="image">
                            <img class="three-image" src="../assets/image3.png">
                            <div class="inkingerier">INKINGERIER</div>
                            <img src="../assets/Vector.png" alt="image" class="painting"></div>

                    </div>

                </div>
            </section>
        </main>
        <footer>
            <section class="footer">
                <div class="footer-body">
                    <div><span class="inst">Inst</span></div>
                    <span>------</span>
                    <div class="fb">Fb</div>

                </div>
            </section>
        </footer>
    </div>

</template>

<script>
    import mainContant from "@/components/mainContant/index";

    export default {
        name: "mainContent",
        // components: {
        //     mainContant
        // }
    };
</script>


<style scoped>
    .drag-me {
        opacity: 0;
    }

    .main-image-container:hover .drag-me {
        opacity: 1;
    }

    @keyframes slidein {
        from {
            margin-left: 50%;
            width: 100%;
        }

        to {
            margin-left: -70%;
            width: 100%;
        }
    }

    .hamburger {
        display: none;
    }

    .inkingerier {
        animation-duration: 3s;
        animation-name: slidein;
        animation-iteration-count: infinite;
        animation-direction: alternate;
        display: flex;
        justify-content: center;
        z-index: 4;
        position: absolute;
        top: 50%;
        /*position: relative;*/
        font-family: Schnyder Cond XL Demi;
        font-size: 125.581px;
        line-height: 86%;
        /* or 108px */

        display: flex;
        align-items: center;
        text-align: center;
        text-transform: uppercase;

        color: #580300;

        mix-blend-mode: darken;
    }

    .footer {
        position: absolute;
        bottom: 0;
    }

    .footer-body {
        display: flex;
    }

    .list {
        padding-right: 20px;
    }

    .inst {
        font-size: 11px;
    }

    .fb {
        font-size: 11px;
        line-height: 2;
        margin-left: 2px;
    }


    .main-image-container {
        position: relative;
    }

    .body-theeImage {
        margin-top: -3vw;
        display: flex;
        justify-content: center;
        margin-left: 35vw;
    }

    .painting {
        position: absolute;
        top: -6vw;
        z-index: -1;
        left: 50%;
        transform: translateX(-50%);
    }

    .three-image {
        object-fit: cover;
        width: 345px;
        height: 238px;
        transform: rotate(2.03deg);
        position: absolute;
        left: calc(100% - 100px);
        bottom: 100px;
    }

    .two-image {
        object-fit: cover;
        /*margin-left: 19vw;*/
        /*margin-top: 8vw;*/
        position: absolute;
        top: 20%;
        right: calc(100% + 20px);
        width: 238px;
        height: 331px;
        z-index: 2;;
        transform: rotate(1.1deg);
    }

    .body-image {
        display: flex;
        justify-content: center;
        transform: rotate(1.5deg);
    }

    .header {
        display: flex;
        justify-content: space-between;
    }

    .main-image {
        display: flex;
        justify-content: center;
        width: 476px;
        height: 702px;
        object-fit: cover;
    }

    .menu {
        text-transform: capitalize;
        display: flex;
        flex-direction: column;
    }

    .title {
        padding-left: 10px;
        letter-spacing: -1px;
        color: #000000;
        font-family: GT America;
        font-style: normal;
        font-weight: bold;
        font-size: 16px;
        line-height: 16px;
    }

    h3 {
        margin: 40px 0 0;
    }

    ul {
        list-style-type: none;
        padding: 0;
    }

    li {
        display: inline-block;
        margin: 0 10px;
    }

    a {
        color: #42b983;
    }

    @media screen and (max-width: 1024px) {
        body {
        }

        .main-image {
            display: flex;
            justify-content: center;
            width: 359px;
            height: 530px;
        }

        .two-image {
            position: absolute;
            top: 20%;
            right: calc(100% + 20px);
            width: 163px;
            height: 226px;
            z-index: 2;
            transform: rotate(1.1deg);
        }

        .three-image {
            width: 234px;
            height: 162px;
            transform: rotate(2.03deg);
            position: absolute;
            left: calc(100% - 100px);
            bottom: 100px;
            object-fit: cover;
        }

        .inkingerier {
            animation-duration: 3s;
            animation-name: slidein;
            animation-iteration-count: infinite;
            animation-direction: alternate;
            display: flex;
            justify-content: center;
            z-index: 4;
            position: absolute;
            top: 50%;
            /*position: relative;*/
            font-family: Schnyder Cond XL Demi;
            font-size: 96px;
            line-height: 86%;
        }
    }

    @media screen and (max-width: 768px) {
        .main-image {
            display: flex;
            justify-content: center;
            width: 359px;
            height: 530px;
        }

        .main-content {
            padding-top: 13vw;
        }

        .painting {
            position: absolute;
            width: 506px;
            height: 605px;
            top: -6vw;
            z-index: -1;
            left: 50%;
            transform: translateX(-50%);
        }
    }

    @media screen and (max-width: 414px) {
        .painting {
            width: 392px;
            height: 493px;
        }

        .main-image {
            width: 273px;
            height: 403px;
        }

        .three-image {
            display: none
        }

        .two-image {
            display: none;

        }

        .inkingerier {
            font-size: 48px;
        }

        .menu {
            display: none
        }

        .footer {
            padding-bottom: 40vw;
        }

        .hamburger {
            display: table-caption;
        }

        . {
            padding-top: 13vw;
        }
    }

    @media screen and (max-width: 375px) {

        .main-image {
            width: 249.67px;
            height: 368.56px;
        }

        .inkingerier {
            font-size: 44px;
        }

        .painting {
            width: 339px;
            height: 429px;
        }
    }
</style>
