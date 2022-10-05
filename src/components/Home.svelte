<script>
    import heroImage from '../assets/images/hero.png'
</script>

<section>
    <div class="hero-titles" id="hero-titles">
        <div class="secondary-title">
            <span>ESTABLISHED IN 1984</span>
        </div>
        <div class="primary-title">
            <div>
                <h1>WE DESIGN FUTURE.</h1>
            </div>
            <div>
                <h1>
                    WE NEED <strong>OKI MOTTO.</strong>
                </h1>
            </div>
        </div>
        <div />
    </div>
    <div />
    <div class="hero-image">
        <img src={heroImage} alt="Large beam Architecture" />
        <div class="white-block">
            <div />
        </div>
    </div>
    <div class="horizontal-lines" />
</section>

<style lang="scss">
    section {
        position: relative;
        .hero-titles {
            margin-top: 4em;
            z-index: 5;
            @media screen and (max-width: 1024px) {
                margin-top: 1em;
            }
            .secondary-title {
                margin-left: 10rem;
                font-size: 1.2rem;

                @media screen and (max-width: 1024px) {
                    margin-left: 2rem;
                    font-size: 1rem;
                }
            }
            .primary-title {
                border-top: 1px #ccc solid;
                h1 {
                    margin-left: 10rem;
                    line-height: 1.1em;
                    font-size: 5rem;
                    strong {
                        color: #00a3ff;
                    }

                    @media screen and (max-width: 1024px) {
                        width: 60%;
                        min-width: 300px;
                        font-size: 3rem;
                        margin-left: 2rem;
                    }
                    @media screen and (max-width: 300px) {
                        font-size: 1rem;
                        min-width: none;
                    }
                }
            }
        }

        .hero-image {
            margin-top: 1em;
            overflow: hidden;
            position: relative;
            z-index: 2;
            img {
                width: 100%;
                height: 720px;
                margin-top: -5em;
                object-fit: cover;
                position: relative;
                @media screen and (max-width: 1024px) {
                    height: 500px;
                }
            }
            .white-block {
                width: 100%;
                height: 200px;
                background-color: white;
                position: absolute;
                top: 200px;
                z-index: 3;
                @media screen and (max-width: 1024px) {
                    top: 100px;
                    height: 100px;
                }
                div {
                    position: absolute;
                    border-left: 1px #ccc solid;
                    border-right: 1px #ccc solid;
                    right: 30%;
                    top: 0;
                    bottom: 0;
                    width: 200px;
                }
            }
        }
        .horizontal-lines {
            width: 200px;
            border-left: 1px #ccc solid;
            border-right: 1px #ccc solid;
            position: absolute;
            bottom: 0;
            top: -500px;
            right: 30%;

            @media screen and (max-width: 1024px) {
                opacity: 0;
            }
        }
    }
</style>
