<script>
    let background = `<svg xmlns="http://www.w3.org/2000/svg" width="146" height="145"><g fill="none" fill-rule="evenodd" stroke="#CFD8EF"><circle cx="63" cy="82" r="62.5"/><circle cx="105" cy="41" r="40.5"/></g></svg>`;
</script>

<style>
    header {
        position: relative;
        text-align: center;
        margin-top: 5vh;
        padding: 5vw
    }

    h1 {
        color: hsl(227, 35%, 25%);
        font-size: 19px;
        font-weight: 800;
    }

    h2 {
        color: lightslategray;
        font-size: 15px;
        padding: 15px 26px;
        line-height: 26px;
    }

    .background-circle {
        position: absolute;
        z-index: -1;
        top: 4vw;
        left: 22vw;
        transform: scale(1.2);
    }

    @media only screen and (min-width: 1440px) {
        header {
            margin-top: -45vh;
        }

        h1 {
            font-size: 2rem;
        }

        h2 {
            font-size: 1.28rem;
            font-weight: 600;
        }

        .background-circle {
            top: 6vw;
            left: 19vw;
            transform: scale(1.3);
        }
    }
</style>

<header>
    <h1>Simple, traffic-based pricing</h1>
    <h2>Sign-up for our 30-day trial. No credit card required.</h2>
    <div class="background-circle">
        {@html background}
    </div>
</header>
