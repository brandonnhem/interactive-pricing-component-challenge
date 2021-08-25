<style>
    .discount {
        display: flex;
        justify-content: center;
        align-items: center;
    }

    .toggle {
        -webkit-appearance: none;
        -moz-appearance: none;
        appearance: none;
        width: 45px;
        height: 20px;
        display: inline-block;
        position: relative;
        border-radius: 50px;
        overflow: hidden;
        outline: none;
        border: none;
        cursor: pointer;
        background-color: hsl(223, 50%, 87%);
        transition: background-color ease 0.3s;
    }

    .toggle:before {
        content: "";
        display: block;
        position: absolute;
        z-index: 2;
        width: 11px;
        height: 11px;
        background: #fff;
        left: 4px;
        top: 4px;
        border-radius: 50%;
        font: 10px/28px Helvetica;
        text-transform: uppercase;
        font-weight: bold;
        text-indent: -22px;
        word-spacing: 37px;
        color: #fff;
        text-shadow: -1px -1px rgba(0,0,0,0.15);
        white-space: nowrap;
        box-shadow: 0 1px 2px rgba(0,0,0,0.2);
        transition: all cubic-bezier(0.3, 1.5, 0.7, 1) 0.3s;
    }

    .toggle:checked {
        background-color: #4CD964;
    }

    .toggle:checked:before {
        left: 32px;
    }

    p {
        color: lightslategray;
    }

    #discount-special {
        font-size: 12px;
        border-radius: 25px;
        padding: 4px 6px;
        background-color: hsl(14, 92%, 95%);
        color: hsl(15, 100%, 70%);
    }
</style>

<div class="discount">
    <p>Monthly Billing</p>
    <label for="Discount">
        <input class="toggle" type="checkbox">
    </label>
    <p>Yearly Billing</p>
    <p id="discount-special">-25%</p>
</div>