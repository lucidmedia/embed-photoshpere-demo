# embedded-photosphere-demo
Sample code that demonstrates how to embed a photo sphere

<a href="https://storage.googleapis.com/static.lucid.media/demos/embedded-photosphere-demo.html">Demo: Webpage with embedded photo sphere.</a>

##### Go to maps.google.com and lookup the business. Then click on the photo sphere. Once open click the veritcal dots next to on the top left of the screen to the right of the photo sphere name. Copy the share code and paste it in a text editor.

```html
https://www.google.com/maps/contrib/111060727942037579956/photos/@40.6186832,-75.3823847,3a,90y,23.36h,91.67t/data=!3m8!1e1!3m6!1s-HmoSAimXqmA%2FVscrY6grPoI%2FAAAAAAAA2t0%2FOZsgjelYZ1k!2e4!3e11!6s%2F%2Flh3.googleusercontent.com%2F-HmoSAimXqmA%2FVscrY6grPoI%2FAAAAAAAA2t0%2FOZsgjelYZ1k%2Fw203-h100-p-k-no%2F!7i8000!8i4000
```
    
##### Delete everything before the 'lh4' or 'lh3' or 'lh{{some number}} and everything after the 'p-k-no'

```html
lh3.googleusercontent.com%2F-HmoSAimXqmA%2FVscrY6grPoI%2FAAAAAAAA2t0%2FOZsgjelYZ1k%2Fw203-h100-p-k-no
```

##### Prepend the following to the url string you have left.

```html
https://ssl.gstatic.com/pano/embed/?bsv&imageurl=https://
```

##### Append the folloing to the url string you have left.

```html
&fullsize=8000,4000&croppedsize=8000,4000&offset=0,0&autorotate=1
```

##### You should be left with a static link to the photo sphere (see if it works by pasting it into the browser)

```html
https://ssl.gstatic.com/pano/embed/?bsv&imageurl=https://lh3.googleusercontent.com%2F-HmoSAimXqmA%2FVscrY6grPoI%2FAAAAAAAA2t0%2FOZsgjelYZ1k%2Fw203-h100-p-k-no&fullsize=8000,4000&croppedsize=8000,4000&offset=0,0&autorotate=1
```

##### Prepend the following to the static link

```html
<iframe src="https://ssl.gstatic.com/pano/embed/?bsv&imageurl=
```

##### Append the folloing to the static link

```html
&fullsize=8000,4000&croppedsize=8000,4000&offset=0,0&autorotate=1" marginwidth="0" marginheight="0" scrolling="no" frameborder="0" height="100%" width="100%"></iframe> 
```
    
##### The final iFrame Code should look like this:

```html
<iframe src="https://ssl.gstatic.com/pano/embed/?bsv&imageurl=https://ssl.gstatic.com/pano/embed/?bsv&imageurl=https://lh3.googleusercontent.com%2F-HmoSAimXqmA%2FVscrY6grPoI%2FAAAAAAAA2t0%2FOZsgjelYZ1k%2Fw203-h100-p-k-no&fullsize=8000,4000&croppedsize=8000,4000&offset=0,0&autorotate=1&fullsize=8000,4000&croppedsize=8000,4000&offset=0,0&autorotate=1" marginwidth="0" marginheight="0" scrolling="no" frameborder="0" height="100%" width="100%"></iframe>
```
    

