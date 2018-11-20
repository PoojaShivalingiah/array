<!DOCTYPE html>
<html>
<head>
	<script src="https://ajax.googleapis.com/ajax/libs/jquery/2.1.1/jquery.min.js"></script>
	<title>Volume Example</title>
</head>
<body>
	<div style="text-align: center;" >
<video width="600" height="500" id="vd"  muted>
	<source src="http://distribution.bbb3d.renderfarming.net/video/mp4/bbb_sunflower_1080p_60fps_normal.mp4" type="video/mp4">
</video>
</div>
<div id="demo" style="text-align: center;">
	<input type="range" name="" id="vol" min="0" max="1" step="0.1" value="1"/>
</div>
</body>
<script type="text/javascript">
	document.getElementById("vd").play();
	$("#vd").on('change', function(){
		$('#vd').prop("vol",this.value);
	});

</script>
</html>
