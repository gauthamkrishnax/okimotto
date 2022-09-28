<script>
    import heroImage from '../assets/images/hero.png'
</script>

<section>
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
        <div class="white-block" />
    </div>
</section>

<style lang="scss">
    .hero-title {
        margin-top: 12em;
        .secondary-title {
            margin-left: 10rem;
            font-size: 1.2rem;
        }
        .primary-title {
            border-top: 1px #eeeeee solid;
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
            margin-top: -5em;
        }
        .white-block {
            width: 100vw;
            height: 150px;
            background-color: white;
            position: absolute;
            top: 200px;
        }
    }
</style>
