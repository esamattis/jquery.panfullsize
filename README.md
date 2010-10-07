
jQuery plugin - Pan full size images
====================================


- Replaces the img-element with an inline-block "pan" div-element with the image as background.
- Syntax: $("img").panFullSize(width, height, callback);
    - Width and height are the dimensions of pan-div.
    - Callback is called when zoom elements has been created.
    - If not set, values will be taken from the img-element or, if already exists, from the pan-div.
    - Normal image view can be restored with normalView().
    - Throws an exception if tried to apply with other than img-element or the created pan-div.
- Tested with Firefox 3.6, Google Chrome 7 and Opera 10.60


Example
-------

    $("img#mypic").panFullSize(700, 450).css("border", "medium solid black");

    $("a#zoom").toggle(function(){
            $("img#mypic").normalView();
        },
        function(){
            $("img#mypic").panFullSize();.
        }
    );



Checkout the demo here:

http://epeli.github.com/jquery.panfullsize/
