

  

<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN">
<html>
 <head>
<script type="text/javascript">
function formSubmit()
{
document.forms["myForm"].submit();
}
</script>
</head>

<body>

<form name="myForm" action="MyHtml.html" method="get">
  First name: <input type="text" name="fname" /><br />
  Last name: <input type="text" name="lname" /><br />
  <input type="button" onclick="formSubmit()" value="Send form data!" />
</form>

<p>请单击确认按钮，输入会发送到服务器上名为 "form_action.asp" 的页面。</p>

</body>
</html>
