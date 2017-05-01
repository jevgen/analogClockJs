# analogClockJs
An analogClock js plug that written by native javascript (jQuery is not required but also campatiable). 

<img src="https://github.com/kenlam0083/analogClockJs/blob/master/demo.png"/>


    <div id="clock">
    </div>

    <script src="analogClock.js"></script>
    
    <script>
        AnalogClock("clock");//simple use
        AnalogClock("clock", { width: 300, bgColor: "#bf0" });//simple option
        AnalogClock("clock", new AnalogClockOption(200, "#eee", "#333"));//using option class to customize

        //base on object use, returns an clock object, can do some further style controll by the returned object.
        var opt = new AnalogClockOption(); opt.width = 100;
        var clock = new AnalogClock("clock", opt);
        clock.panel.style.border = "solid 1px red";
    </script>
