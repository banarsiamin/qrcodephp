# qrcodephp
Simple php Qr code ganrator
include('qrcodeclass.php');
$content ='AMIN KHAN BANARSi INDORE banarsiamin@gmail.com ';
$size='40';
$margin='10';
$svg = \banarsiamin\QRcode::svg( $content, false, false, $size, $margin ) ;
		$svg = str_replace( "\n", '', $svg ) ;
		$svg = 'data:image/svg+xml;base64,' . base64_encode( $svg ) ;
		echo "<img src='$svg' />" ;

die;
