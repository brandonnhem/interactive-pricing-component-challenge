<script>
    import Slider from './Slider.svelte';
    import Switch from './Switch.svelte';
</script>

<style>
    h2 {
        color: hsl(225, 20%, 60%);
        font-weight: 800;
        letter-spacing: 2px;
        font-size: 15px;
    }

    .card {
        background-color: white;
        padding: 5vw;
        border-radius: 10px;
        box-shadow: 0 4px 8px 0 rgba(0,0,0,0.2);
        transition: 0.3s;
        text-align: center;
    }

    #trial-btn {
        background-color: hsl(227, 35%, 25%);
        border: none;
        border-radius: 25px;
        padding: 0.8rem 3rem;
        color: hsl(226, 100%, 87%);
        font-weight: 800;
        font-family: 'Manrope', sans-serif;
        cursor: pointer;
    }

    hr {
        margin-left: -5vw;
        width: 83.5vw;
    }

    .row {
        display: flex;
        flex-direction: row;
        justify-content: center;
        align-items: center;
    }

    p {
        color: lightslategray;
        padding: 0 8px;
        margin: 5px;
    }

    .perks {
        margin: 3vh;
    }

    svg {
        transform: scale(1.3);
    }
</style>

<main>
	<div class="card">
        <h2>100K PAGEVIEWS</h2>
        <Slider/>
        <Switch/>        

        <hr>

        <div class="perks">
            <div class="row">
                <svg xmlns="http://www.w3.org/2000/svg" width="9" height="8"><path fill="none" stroke="#10D8C4" stroke-width="2" d="M1 4.134l1.907 1.908L7.949 1"/></svg>
                <p>Unlimited websites</p>
            </div>
            <div class="row">
                <svg xmlns="http://www.w3.org/2000/svg" width="9" height="8"><path fill="none" stroke="#10D8C4" stroke-width="2" d="M1 4.134l1.907 1.908L7.949 1"/></svg>
                <p>100% data ownership</p>
            </div>
            <div class="row">
                <svg xmlns="http://www.w3.org/2000/svg" width="9" height="8"><path fill="none" stroke="#10D8C4" stroke-width="2" d="M1 4.134l1.907 1.908L7.949 1"/></svg>
                <p>Email reports</p>
            </div>
        </div>

        <button id="trial-btn">
            Start my trial
        </button>
    </div>
</main>