#handle.js

##About

handle.js is thin wrapper of event handling.

##Usage

    var foo = new Handle(document.querySelectorAll("#id .className"));
    var bar = new Handle(document.querySelectorAll("#id"));
    var eventHandler = function() {
    	console.log("log");
    };

    foo.bind("click", eventHandler);
    
    foo.unbind("click", eventHandler)
    
    bar.delegate("click", ".className", eventHandler);
    
    bar.undelegate("click", ".className", eventHandler);
    bar.undelegate("click", ".className");
    bar.undelegate("click");

##License

Copyright [1000ch.net](http://1000ch.net/)  
Released under the MIT license  