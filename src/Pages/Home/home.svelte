<script lang="ts">
</script>

<header>
    <div class="leftSide"><span>THE NEUES</span></div>
    <div class="rightSide">
        <span>BUY TICKETS</span>
        <span>OUR STORY</span>
        <span>CONTACT</span>
    </div>
</header>
<section>
    <div class="grid">
        <div class="leftSec">
            <div class="title">NEUES MUSEUM</div>
            <div class="descriptions">
                <div>
                    Mauris porttitor mauris ut aliquet viverra. Sed tincidunt augue nec nunc fermentum congue.
                    Pellentesque eu imperdiet elit. Ut et posuere justo, lobortis finibus lacus. Donec quis accumsan
                    risus, a ultricies nisl.
                </div>
                <div>
                    Maecenas luctus convallis sapien, at luctus orci pulvinar in. Pellentesque finibus quis risus sit
                    amet mattis. Vestibulum id eros sagittis, sollicitudin dolor sed, venenatis ex. Praesent ut ipsum ac
                    nibh lobortis ultrices at ut ex.
                </div>
            </div>
            <div class="next">Buy your Tickets --></div>
        </div>
        <div class="rightSec">
            <div class="year">2022</div>
            <div class="img"><img src={'imgs/IMG.jpg'} /></div>
        </div>
    </div>
</section>

<style lang="scss">
    header {
        display: flex;
        justify-content: space-between;
        font-weight: 300;

        & > div {
            display: flex;
            height: 100%;
            font-size: 1.6rem;

            justify-content: center;
            align-items: center;
            padding: 1rem;

            span {
                padding: 1rem;
            }
        }
    }

    section {
        display: flex;

        /* height: 100%;
        width: 100%; */

        .grid {
            display: grid;
            grid-template-columns: 50% 50%;
            justify-content: center;
            align-items: center;
            padding: 2rem 4em;
            box-sizing: border-box;
            /* padding-right: 2rem; */

            .leftSec {
                display: flex;
                flex-direction: column;
                justify-content: space-between;
                align-items: center;
                height: 100%;

                .title {
                    display: flex;
                    justify-content: center;
                    align-items: center;
                    font-size: 10rem;
                    font-weight: 600;
                }

                .descriptions {
                    display: grid;
                    grid-template-columns: 50% 50%;
                    justify-content: center;

                    * {
                        text-align: justify;
                        padding: 1rem;
                        line-height: 1.7;
                        font-size: 1.15rem;
                    }
                }

                .next {
                    font-weight: 600;
                    font-size: 1.2rem;
                    border-bottom: white 2px solid;

                    &:hover {
                        border-bottom: black 2px solid;
                        cursor: pointer;
                    }
                }
            }

            .rightSec {
                display: flex;
                justify-content: flex-end;
                /* align-items: center; */

                height: 100%;

                .year {
                    height: fit-content;
                    margin-top: 2rem;
                    font-size: 2.2rem;
                    font-weight: 100;
                    transform: rotateZ(-90deg);
                    height: 1rem;
                }

                .img {
                    display: flex;
                    height: 100%;

                    img {
                        height: 80vh;
                    }
                }
            }
        }
    }
</style>
