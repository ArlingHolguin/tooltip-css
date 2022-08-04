# Cajero Automatico con JavaScript
### Hola 👋, ToolTips css <img src='https://github.githubassets.com/images/mona-loading-default.gif' alt='github' height='30'>
[Link del Proyecto](https://arlingholguin.github.io/cajero/)  
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

# HTML
<pre><code>
<div class="tool top">Tool Top
    <span class="tiptext hvr-bounce-in">Texto del tool top<a href="http://hola.com">Hola</a></span>
</div>
<button class="tool right">Top right
    <span class="tiptext hvr-bounce-in">Texto del tool right <a href="https://link.com">Link</a></span>
</button>
<button class="tool bottom">tool bottom
    <span class="tiptext hvr-bounce-in">Texto del tool bottom <a href="https://link.com">Link</a></span>
</button>
<div class="tool left">
    <svg xmlns="http://www.w3.org/2000/svg" x="0px" y="0px" width="20" height="20"
        viewBox="0 0 24 24" style=" fill:#000000;">
        <path
            d="M 7.5 1 C 6.6274862 1 5.7932031 1.1755485 5.0332031 1.4882812 L 3.6445312 2.0585938 L 7.5859375 6 L 6 7.5859375 L 2.0585938 3.6445312 L 1.4882812 5.0332031 C 1.1755484 5.7932031 1 6.6274862 1 7.5 C 1 11.078268 3.9217323 14 7.5 14 C 8.11867 14 8.6809561 13.816598 9.2480469 13.654297 L 18.15625 22.560547 C 18.734417 23.138714 19.699176 23.138714 20.277344 22.560547 L 22.5625 20.273438 C 23.136532 19.696462 23.137552 18.731255 22.560547 18.154297 L 13.654297 9.2480469 C 13.816352 8.6810027 14 8.1186541 14 7.5 C 14 3.9217323 11.078268 1 7.5 1 z M 7.5 3 C 9.9977323 3 12 5.0022677 12 7.5 C 12 8.1069469 11.878016 8.6818072 11.660156 9.2128906 L 11.408203 9.8300781 L 20.792969 19.214844 L 19.216797 20.792969 L 9.8300781 11.40625 L 9.2128906 11.660156 C 8.6825114 11.878548 8.1081276 12 7.5 12 C 5.0022677 12 3 9.9977323 3 7.5 C 3 7.47441 3.0132432 7.4532073 3.0136719 7.4277344 L 6 10.414062 L 10.414062 6 L 7.4277344 3.0136719 C 7.4532073 3.0132432 7.47441 3 7.5 3 z">
        </path>
    </svg>
    <span class="tiptext hvr-bounce-in">Texto del tool left</span>
</div>
</code></pre>
