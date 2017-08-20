# converter-CRC32-MD5-SHA1
<!DOCTYPE html>
<html>
<head>
	<title>Convert Text to Crc32, md5 and Sha1</title>
</head>
<body>
<center>
	<div style="border:5px solid #888; width:350px; padding:20px;">
		<form method="post">
			<h3>Convert Text to Crc32, md5 and Sha1</h3><br>
				<input type="text" name="convert" style="padding:5px; width:245px;" placeholder="Type Anything....">
				<input type="submit" name="con" value="Convert" style="padding:5px;">
		</form>
		<br>
			<span><b>Crc32 Result</b></span><br>
				<input type="text" value="<?php if(isset($_POST['con'])){ echo crc32($_POST['convert']); } ?>" style="padding:5px; width:310px; " readonly><br><br>
			
			<span><b>Md5 Result</b></span><br>
				<input type="text" value="<?php if(isset($_POST['con'])){ echo md5($_POST['convert']); } ?>" style="padding:5px; width:310px; " readonly><br><br>
			
			<span><b>Sha1 Result</b></span><br>
				<input type="text" value="<?php if(isset($_POST['con'])){ echo sha1($_POST['convert']); } ?>" style="padding:5px; width:310px; " readonly><br><br>
	</div>
</center>
</body>
</html>

