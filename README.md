# Tooltips con css y html
### Hola 👋, ToolTips css <img src='https://github.githubassets.com/images/mona-loading-default.gif' alt='github' height='30'>
[Link del Proyecto](https://arlingholguin.github.io/tooltip-css/)  
<h3 align="left">Support:</h3>
<p><a href="https://www.buymeacoffee.com/arling"> <img align="left" src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" height="50" width="210" alt="https://www.buymeacoffee.com/arling" /></a></p><br><br>

###
# css
<pre><code>
/* tolptip  */
        .tool {
            position: relative;
            display: inline-block;
            /* border-bottom: 1px dotted black; */
            cursor: pointer;

        }

        .tool .tiptext {
            visibility: hidden;
            width: 150px;
            background-color: #124256;
            color: #fff;
            text-align: center;
            font-size: 11px;
            border-radius: 3px;
            padding: 6px 0;
            position: absolute;
            z-index: 1;
            box-shadow: 0 5px 10px rgba(0, 0, 0, 0.3);
            cursor: pointer;
        }

        .tool .tiptext::after {
            content: "";
            position: absolute;
            border-width: 5px;
            border-style: solid;
        }

        .tool:hover .tiptext {
            visibility: visible;
        }

        /* toltip top  */
        .tool.top .tiptext {
            margin-left: -60px;
            bottom: 150%;
            left: 50%;
        }

        .tool.top .tiptext::after {
            margin-left: -5px;
            top: 100%;
            left: 50%;
            border-color: #124256 transparent transparent transparent;
        }

        /* tool abajo  */
        .tool.bottom .tiptext {
            margin-left: -60px;
            top: 150%;
            left: 50%;
        }

        .tool.bottom .tiptext::after {
            margin-left: -5px;
            bottom: 100%;
            left: 50%;
            border-color: transparent transparent #124256 transparent;
        }

        /* tool izquierda */
        .tool.left .tiptext {
            top: -5px;
            right: 110%;
        }

        .tool.left .tiptext::after {
            margin-top: -5px;
            top: 50%;
            left: 100%;
            border-color: transparent transparent transparent #124256;
        }

        /* tool derecha  */
        .tool.right .tiptext {
            top: -5px;
            left: 110%;
        }

        .tool.right .tiptext::after {
            margin-top: -5px;
            top: 50%;
            right: 100%;
            border-color: transparent #124256 transparent transparent;
        }

/*hover*/
/* Bounce In */

.hvr-bounce-in {
    display: inline-block;
    vertical-align: middle;
    -webkit-transform: perspective(1px) translateZ(0);
    transform: perspective(1px) translateZ(0);
    box-shadow: 0 0 1px rgba(0, 0, 0, 0);
    -webkit-transition-duration: 0.5s;
    transition-duration: 0.5s;
}

.hvr-bounce-in:hover,
.hvr-bounce-in:focus,
.hvr-bounce-in:active {
    -webkit-transform: scale(1.2);
    transform: scale(1.2);
    -webkit-transition-timing-function: cubic-bezier(0.47, 2.02, 0.31, -0.36);
    transition-timing-function: cubic-bezier(0.47, 2.02, 0.31, -0.36);
}

</code></pre>


