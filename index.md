// Прокрутка страницы 
    $(window).scroll(function () {
        var goTop = $("#go-top");
        if ($(this).scrollTop() > 200) {
            goTop.fadeIn();
        } else {
            goTop.fadeOut();
        }
    });
    $('#go-top a').click(function () {
        $('html, body').animate({
            scrollTop: 0
        }, 800);
        return false;
    });
<form method="get" action="http://www.bing.com/search">
<div style="border:1px solid black;padding:4px;width:20em;">
  <table border="0" align="center" cellpadding="0">
  <tr><td>
  <input type="text"   name="q" size="25"
  maxlength="255" value="" />
  <input type="submit" value="Bing Search" /></td></tr>
  <tr><td align="center" style="font-size:75%">
  <input type="radio"  name="q1" value="" />The Web
  <input type="radio"  name="q1"
  value="site:yoursite.com" /> Only Your Site<br />
  </td></tr></table>
  </div>
</form>



