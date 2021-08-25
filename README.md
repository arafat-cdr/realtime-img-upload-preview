# realtime-img-upload-preview

```html
<!DOCTYPE html>
<html lang="en">
<head>
	<meta charset="UTF-8">
	<meta name="viewport" content="width=device-width, initial-scale=1.0">
	<title>Document</title>
</head>
<body>
	<input type="file" id="userImgUpload">
	<img src="#" alt="img" id="userImg">
	<script>
		// real time image update the img path
		userImgUpload.onchange = evt => {
		  const [file] = userImgUpload.files
		  if (file) {
		    userImg.src = URL.createObjectURL(file)
		  }
		}
		// end real time img update path
	</script>
</body>
</html>
```
