<script>
    import heroImage from '../assets/images/hero.png'
</script>

<section class="home">
    <div class="hero-title">
        <div class="secondary-title">ESTABLISHED IN 1984</div>
        <div class="primary-title">
            <div><h1>WE DESIGN FUTURE.</h1></div>
            <div><h1>WE NEED <strong>OKI MOTTO.</strong></h1></div>
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
    .home {
        position: relative;
        .horizontal-lines {
            width: 200px;
            border-left: 1px #ccc solid;
            border-right: 1px #ccc solid;
            position: absolute;
            bottom: 0;
            top: -200px;
            right: 30%;
            z-index: -1;
        }
    }
    .hero-title {
        margin-top: 12em;
        .secondary-title {
            margin-left: 10rem;
            font-size: 1.2rem;
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
            }
        }
    }

    .hero-image {
        margin-top: 1em;
        overflow: hidden;
        position: relative;
        img {
            width: 100%;
            height: 720px;
            margin-top: -5em;
            object-fit: cover;
            position: relative;
        }
        .white-block {
            width: 100%;
            height: 200px;
            background-color: white;
            position: absolute;
            top: 200px;
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
</style>
