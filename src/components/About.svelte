<script>
    import AboutImage from '../assets/images/about.png'
</script>

<section>
    <div class="about1">
        <p>
            Widely considered one of the world’s most innovative architects, Oki
            Motto is known for his continued exploration of post-modernism and
            its role in contemporary architecture with respect to form-finding.
        </p>
    </div>
    <div class="about2">
        <p>
            Found by Architects Taha Sinouyi and Shay Mick, Okii Moto traslates
            from Japanese to big base.
        </p>
    </div>
    <div class="about3">
        <div class="div1" />
        <article class="div2">
            <h2>ARC<br />HITE<br />CTURE</h2>
            <p>
                In the material form of buildings, we are perceived as cultural
                symbols and as works of art. It is both the process and the
                product of sketching, conceiving, planning, designing, and
                constructing buildings or other structures.
            </p>
        </article>
        <div class="div3" />
        <div class="div4" />
        <article class="div5">
            <h2>DE<br />SIGN</h2>
            <p>
                Plan or specification for the construction of an object or
                system or for the implementation of an activity or process or
                the result of that plan or specification in the form of a
                prototype, product, or process.
            </p>
        </article>
        <div class="div6" />
    </div>
    <div class="about4">
        <img src={AboutImage} alt="" />
    </div>
</section>

<style lang="scss">
    section {
        display: grid;
        grid-template-columns: 2fr 1fr;
        grid-template-rows: 1fr 2fr;
        grid-column-gap: 0px;
        grid-row-gap: 0px;
        @media screen and (max-width: 1024px) {
            display: grid;
            grid-template-columns: 1fr;
            grid-template-rows: repeat(2, 0.5fr) repeat(2, 2fr);
            grid-column-gap: 0px;
            grid-row-gap: 0px;
        }
    }

    .about1 {
        grid-area: 1 / 1 / 2 / 2;
        display: flex;
        justify-content: flex-end;
        align-items: center;
        @media screen and (max-width: 1024px) {
            grid-area: 1 / 1 / 2 / 2;
            display: block;
            padding: 2em;
            margin-top: 4em;
        }
        p {
            text-align: right;
            max-width: 450px;
            margin-right: 1em;
            margin-bottom: 4em;
            @media screen and (max-width: 1024px) {
                text-align: left;
            }
        }
    }
    .about2 {
        grid-area: 1 / 2 / 2 / 3;
        display: flex;
        justify-content: flex-start;
        align-items: center;
        @media screen and (max-width: 1024px) {
            grid-area: 2 / 1 / 3 / 2;
            justify-content: flex-end;
            align-items: flex-end;
        }
        p {
            max-width: 250px;
            margin-left: 1em;
            margin-top: 4em;
            @media screen and (max-width: 1024px) {
                margin: 0;
                margin-right: 2em;
                margin-bottom: 3em;
                text-align: right;
            }
        }
    }
    .about3 {
        grid-area: 2 / 1 / 3 / 2;
        display: grid;
        grid-template-columns: 1fr 3fr 0.3fr;
        grid-template-rows: repeat(2, 1fr);
        grid-column-gap: 0px;
        grid-row-gap: 0px;
        @media screen and (max-width: 1024px) {
            grid-area: 3 / 1 / 4 / 2;
            display: grid;
            grid-template-columns: 0.1fr 1fr 0.1fr;
            grid-template-rows: repeat(2, 1fr);
            grid-column-gap: 0px;
            grid-row-gap: 0px;
        }
        h2 {
            font-size: 4rem;
            line-height: 1em;
            letter-spacing: 0.2em;
        }
        p {
            max-width: 500px;
            margin-top: 1em;
        }

        .div1 {
            grid-area: 1 / 1 / 2 / 2;
            border-top: 1px solid #ccc;
            border-right: 1px solid #ccc;
            @media screen and (max-width: 1024px) {
                grid-area: 1 / 1 / 2 / 2;
            }
        }
        .div2 {
            grid-area: 1 / 2 / 2 / 3;
            border-top: 1px solid #ccc;
            border-right: 1px solid #ccc;
            padding: 1em;
            @media screen and (max-width: 1024px) {
                grid-area: 1 / 2 / 2 / 3;
            }
        }
        .div3 {
            grid-area: 1 / 3 / 2 / 4;
            border-top: 1px solid #ccc;
            @media screen and (max-width: 1024px) {
                grid-area: 1 / 3 / 2 / 4;
            }
        }
        .div4 {
            grid-area: 2 / 1 / 3 / 2;
            border-top: 1px solid #ccc;
            border-right: 1px solid #ccc;
            @media screen and (max-width: 1024px) {
                grid-area: 2 / 1 / 3 / 2;
            }
        }
        .div5 {
            grid-area: 2 / 2 / 3 / 3;
            border-top: 1px solid #ccc;
            border-right: 1px solid #ccc;
            text-align: right;
            padding: 1em;
            p {
                float: right;
            }
            @media screen and (max-width: 1024px) {
                grid-area: 2 / 2 / 3 / 3;
            }
        }
        .div6 {
            grid-area: 2 / 3 / 3 / 4;
            border-top: 1px solid #ccc;
            @media screen and (max-width: 1024px) {
                grid-area: 2 / 3 / 3 / 4;
            }
        }
    }
    .about4 {
        grid-area: 2 / 2 / 3 / 3;
        overflow: hidden;
        @media screen and (max-width: 1024px) {
            grid-area: 4 / 1 / 5 / 2;
        }
        img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }
    }
</style>
