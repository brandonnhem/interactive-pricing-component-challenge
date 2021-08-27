<script>
    let range = 16;

    function handleSlide() {
        range = this.value;
    }
</script>

<style>
    .rangeslider {
        width: 100%;
    }

    .slider {
        -webkit-appearance: none;
        background: hsl(174, 77%, 80%);
        width: 100%;
        height: 12px;
        opacity: 2;
        border-radius: 25px;
    }

    input[type=range]::-webkit-slider-thumb {
        -webkit-appearance: none;
        height: 40px;
        width: 40px;
        border-radius: 50%;
        background: hsl(174, 86%, 45%);
        background-image: url(../images/icon-slider.svg);
        background-repeat: no-repeat;
        background-position: center;
        cursor: pointer;
    }

    input[type=range]::-moz-range-thumb {
        -webkit-appearance: none;
        height: 40px;
        width: 40px;
        border-radius: 50%;
        background: hsl(174, 86%, 45%);
        background-image: url(../images/icon-slider.svg);
        background-repeat: no-repeat;
        background-position: center;
        cursor: pointer;
    }

    input[type=range]::-ms-thumb {
        -webkit-appearance: none;
        height: 40px;
        width: 40px;
        border-radius: 50%;
        background: hsl(174, 86%, 45%);
        background-image: url(../images/icon-slider.svg);
        background-repeat: no-repeat;
        background-position: center;
        cursor: pointer;
    }

    .price {
        display: flex;
        justify-content: center;
        align-items: center;
    }

    #big-money {
        color: hsl(227, 35%, 25%);
        font-size: 2rem;
        font-weight: 800;
    }

    #month {
        margin-left: 0.5rem;
        color: hsl(225, 20%, 60%);
    }

    @media only screen and (min-width: 1440px) {
        .price {
            position: absolute;
            top: 1vh;
            left: 28vw;
        }

        #big-money {
            font-size: 3rem;
        }

        #month {
            font-size: 1.5rem;
        }

        .slider {
            margin-top: 4vh;
        }
    }
</style>

<div class="rangeslider">
    <label for="sliderRange">
        <input type="range" min="1" max="32" value="16" class="slider" id="sliderRange" on:input={handleSlide} aria-label="range slider">
    </label>
    <div class="price">
        <p id="big-money">${range.toString() + '.00'}</p>
        <p id="month">/ month</p>
    </div>

</div>