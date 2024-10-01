<script>
    // No script needed for this simple example
</script>

<style>
    .hexagon {
        width: 100px;
        height: 55px;
        background-color: red;
        position: relative;
    }

    .hexagon:before,
    .hexagon:after {
        content: "";
        position: absolute;
        width: 0;
        border-left: 50px solid transparent;
        border-right: 50px solid transparent;
    }

    .hexagon:before {
        bottom: 100%;
        border-bottom: 27.5px solid red;
    }

    .hexagon:after {
        top: 100%;
        width: 0;
        border-top: 27.5px solid red;
    }

    .container {
        display: flex;
        justify-content: center;
        align-items: center;
        height: 100vh;
    }
</style>

<div class="container">
    <div class="hexagon"></div>
</div>