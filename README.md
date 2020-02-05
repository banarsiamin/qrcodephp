# qrcodephp
Simple php Qr code ganrator
<pre>
include('qrcodeclass.php');<br>

$content ='AMIN KHAN BANARSi INDORE banarsiamin@gmail.com ';<br>


$size='40';<br>

$margin='10';<br>

$svg = \banarsiamin\QRcode::svg( $content, false, false, $size, $margin ) ;<br>

$svg = str_replace( "\n", '', $svg ) ;<br>

$svg = 'data:image/svg+xml;base64,' . base64_encode( $svg ) ;<br>

echo "<img src='$svg' />" ;<br>

die;

</pre>
