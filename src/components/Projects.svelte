<script>
    import AdImage from '../assets/images/ad.png'
</script>

<section>
    <div class="div1">
        <h3>Architectural Design</h3>
        <div>
            <img src={AdImage} alt="" />
        </div>
        <p>
            Our Expert team of Architects provides the best service of post
            modernist and suited architecture through weighted planning and
            precisions. We try to Implement the innovation right out of the box
            while undergoing several researches to <span class="nowrap">
                make the box and contribute to the field.</span
            >
        </p>
    </div>
    <div class="div2">
        <ul>
            <li class="active">Architectural Design</li>
            <li>Interior Design</li>
            <li>Urban Design and Planning</li>
            <li>Solution</li>
        </ul>
    </div>
</section>

<style lang="scss">
    section {
        background-color: #000;
        color: #fff;
        min-height: 110vh;

        display: grid;
        grid-template-columns: 3fr 2fr;
        grid-template-rows: 1fr;
        grid-column-gap: 0px;
        grid-row-gap: 0px;
        // display: none;
        @media screen and (max-width: 1024px) {
            display: grid;
            grid-template-columns: 1fr;
            grid-template-rows: 2fr 1fr;
            grid-column-gap: 0px;
            grid-row-gap: 0px;
        }
        .div1 {
            height: 100%;
            grid-area: 1 / 1 / 2 / 2;
            display: flex;
            justify-content: center;
            text-align: right;
            flex-direction: column;
            padding-left: 30%;
            padding-bottom: 8em;
            padding-top: 12em;
            padding-right: 0.5em;
            border-right: 1px #333 solid;
            @media screen and (max-width: 1024px) {
                grid-area: 1 / 1 / 2 / 2;
                text-align: left;
                padding: 4em 2em 1em 2em;
            }

            h3 {
                font-size: 2em;
                text-align: left;
                margin-bottom: 0.5em;
            }
            img {
                width: 100%;
                // height: 350px;
                object-fit: cover;
                display: inline;
                margin-right: -0.5em;
                @media screen and (max-width: 1024px) {
                    width: 80%;
                    margin-right: 0;
                }
            }
            p {
                max-width: 70%;
                font-size: 0.8em;
                margin-left: auto;
                margin-top: 0.5em;
                @media screen and (max-width: 1024px) {
                    margin-left: 0;
                }
            }
        }
        .div2 {
            grid-area: 1 / 2 / 2 / 3;
            display: flex;
            justify-content: center;
            align-items: center;
            @media screen and (max-width: 1024px) {
                grid-area: 2 / 1 / 3 / 2;
            }
            ul {
                li {
                    font-family: 'Satoshi', sans-serif;
                    list-style: none;
                    text-align: right;
                    color: #aaaaaa;
                    margin-bottom: 0.5em;
                }
                li.active {
                    font-size: 1.5rem;
                    color: #fff;
                }
            }
        }
    }
</style>
