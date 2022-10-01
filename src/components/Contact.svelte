<script>
    import ContactImage from '../assets/images/contact.png'
</script>

<section>
    <div class="div1">
        <h3>Contact</h3>
        <p>Get all information about Oki Motto.</p>

        <form
            accept-charset="UTF-8"
            action="action_page.php"
            autocomplete="off"
            method="GET"
            target="_blank"
        >
            <label for="name">Name:</label><br />
            <input name="name" type="text" placeholder="Enter your Name" />
            <br />
            <label for="name">Email:</label><br />
            <input name="name" type="email" placeholder="abc@domain.com" />
            <br />
            <label for="name">GSM Number:</label><br />
            <input
                name="name"
                type="tel"
                placeholder="Country Code + 0091 0929 30"
            /> <br />
            <button type="submit" value="Submit">Send to Oki Motto</button>
        </form>
    </div>
    <div class="footer-img">
        <img src={ContactImage} alt="" />
    </div>
</section>

<style lang="scss">
    section {
        min-height: 100vh;
        position: relative;
        display: flex;
        align-items: flex-end;
        background-color: #ffffff;
        opacity: 1;
        background-image: linear-gradient(#e7e7e7 3.2px, transparent 3.2px),
            linear-gradient(90deg, #e7e7e7 3.2px, transparent 3.2px),
            linear-gradient(#e7e7e7 1.6px, transparent 1.6px),
            linear-gradient(90deg, #e7e7e7 1.6px, #ffffff 1.6px);
        background-size: 80px 80px, 80px 80px, 16px 16px, 16px 16px;
        background-position: -3.2px -3.2px, -3.2px -3.2px, -1.6px -1.6px,
            -1.6px -1.6px;
        .div1 {
            margin-left: 30%;
            margin-right: 10em;
            z-index: 2;
            width: 100%;
            @media screen and (max-width: 1024px) {
                margin-left: 2em;
                margin-right: 2em;
            }
            h3 {
                font-size: 2em;
            }
            form {
                margin-top: 1em;
                padding: 4em 5em 10em;
                background-color: #f0f0f0;
                @media screen and (max-width: 1024px) {
                    padding: 4em 2em 10em;
                }
                label {
                    font-family: 'Satoshi', sans-serif;
                    margin-bottom: 1em;
                }
                input {
                    width: 100%;
                    max-width: 500px;
                    border: none;
                    margin-bottom: 2em;
                    background-color: #000;
                    padding: 0.2em 1em;
                    caret-color: #fff;
                    color: #fff;
                    input::placeholder {
                        color: #bbb;
                    }
                    &[type='text'] {
                        max-width: 300px;
                    }
                }

                button {
                    background-color: #000;
                    color: #fff;
                    border: none;
                    padding: 0.2em 1em;
                    font-family: 'Satoshi', sans-serif;
                    cursor: pointer;
                }
            }
        }

        .footer-img {
            position: absolute;
            bottom: 0;
            left: 0;
            right: 0;

            img {
                width: 100%;
                height: 250px;
                object-fit: cover;
            }
        }
    }
</style>
