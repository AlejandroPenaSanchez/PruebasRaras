<template>
    <div id="Terminal">
        <p>
        -------------------------------------------------------------------------------------
        </p>
        <!-- <pre>
               _    _       _                 _                   _____                   _             _ 
              / \  | | ___ (_) __ _ _ __   __| |_ __ ___    ___  |_   _|__ _ __ _ __ ___ (_)_ __   __ _| |
             / _ \ | |/ _ \| |/ _` | '_ \ / _` | '__/ _ \  / __|   | |/ _ \ '__| '_ ` _ \| | '_ \ / _` | |
            / ___ \| |  __/| | (_| | | | | (_| | | | (_) | \__ \   | |  __/ |  | | | | | | | | | | (_| | |
           /_/   \_\_|\___|/ |\__,_|_| |_|\__,_|_|  \___/  |___/   |_|\___|_|  |_| |_| |_|_|_| |_|\__,_|_|
                         |__/                                                                                                                                    
        </pre> -->
        <p>
        -------------------------------------------------------------------------------------
        </p>
        <div id="input-line" class="input-line">
            <div class="prompt">root@localhost:~#</div>
            <div>
                <input class="cmdline" autofocus />
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'Terminal'
    }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
    #Terminal {
        width: 100%;
        height: 100%;
        margin: 0;
        background-color: black;
        color: greenyellow;
        font: 1.2rem Inconsolata, monospace;
        align-items: left;
    }

    .cmdline {
        outline: none;
        background-color: transparent;
        margin: 0;
        width: 100%;
        font: inherit;
        border: none;
        color: inherit;
    }

    .input-line {
        display: -webkit-box;
        -webkit-box-orient: horizontal;
        -webkit-box-align: stretch;
        display: -moz-box;
        -moz-box-orient: horizontal;
        -moz-box-align: stretch;
        display: box;
        box-orient: horizontal;
        box-align: stretch;
        clear: both;
    }

    .input-line > div:nth-child(2) {
        -webkit-box-flex: 1;
        -moz-box-flex: 1;
        box-flex: 1;
    }
     .prompt {
        white-space: nowrap;
        margin-right: 7px;
        display: -webkit-box;
        -webkit-box-pack: center;
        -webkit-box-orient: vertical;
        display: -moz-box;
        -moz-box-pack: center;
        -moz-box-orient: vertical;
        display: box;
        box-pack: center;
        box-orient: vertical;
        -webkit-user-select: none;
        -moz-user-select: none;
        user-select: none;
    }

    

</style>