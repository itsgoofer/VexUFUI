<script>
    import { SerialPort } from "tauri-plugin-serialplugin";
    // Example: Listing available serial ports
    async function listPorts() {
        let availablePorts = await SerialPort.available_ports();
        console.log("ports: ", availablePorts);
    }

    listPorts();
</script>

<div class="container">
</div>

<style>


    :root {
        font-family: Inter, Avenir, Helvetica, Arial, sans-serif;
        font-size: 16px;
        line-height: 24px;
        font-weight: 400;

        color: #0f0f0f;
        background-color: #f6f6f6;

        font-synthesis: none;
        text-rendering: optimizeLegibility;
        -webkit-font-smoothing: antialiased;
        -moz-osx-font-smoothing: grayscale;
        -webkit-text-size-adjust: 100%;
    }

    .container {
        margin: 0;
        padding-top: 10vh;
        display: flex;
        flex-direction: column;
        justify-content: center;
        text-align: center;
    }


    a {
        font-weight: 500;
        color: #646cff;
        text-decoration: inherit;
    }


    @media (prefers-color-scheme: dark) {
        :root {
            color: #f6f6f6;
            background-color: #2f2f2f;
        }

    }
</style>
