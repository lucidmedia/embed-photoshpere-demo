# embedded-photoshpere-demo
Sample code that demonstrates how to embed a photoshpere

Code from share and embed link on google maps:

<code>https://www.google.com/maps/contrib/111060727942037579956/photos/@40.6041421,-75.4593964,3a,75y,255.25h,90t/data=!3m8!1e1!3m6!1s-5jMaNpghETg%2FVqef77Ks6OI%2FAAAAAAAA2GA%2FswPwG1NqgGk!2e4!3e11!6s%2F%2Flh4.googleusercontent.com%2F-5jMaNpghETg%2FVqef77Ks6OI%2FAAAAAAAA2GA%2FswPwG1NqgGk%2Fw203-h100-p-k-no%2F!7i8000!8i4000 </code>
    
After descecting url:

<!--// lh4.googleusercontent.com%2F-5jMaNpghETg%2FVqef77Ks6OI%2FAAAAAAAA2GA%2FswPwG1NqgGk%2Fw203-h100-p-k-no //-->
    
iFrame Code:

<!--// <iframe src="https://ssl.gstatic.com/pano/embed/?bsv&imageurl={{static photoshpere url}}&fullsize=8000,4000&croppedsize=8000,4000&offset=0,0&autorotate=1" marginwidth="0" marginheight="0" scrolling="no" frameborder="0" height="100%" width="100%"></iframe> //-->
    
New static photosphere static url:

<!--// https://ssl.gstatic.com/pano/embed/?bsv&imageurl=https://lh4.googleusercontent.com/-5jMaNpghETg/Vqef77Ks6OI/AAAAAAAA2GA/swPwG1NqgGk/g/w212-h106-n-k-no&fullsize=8000,4000&croppedsize=8000,4000&offset=0,0&autorotate=1 //->
    
    
Final iFrame Code

<!-- <iframe src="https://ssl.gstatic.com/pano/embed/?bsv&imageurl=https://ssl.gstatic.com/pano/embed/?bsv&imageurl=https://lh4.googleusercontent.com/-5jMaNpghETg/Vqef77Ks6OI/AAAAAAAA2GA/swPwG1NqgGk/g/w212-h106-n-k-no&fullsize=8000,4000&croppedsize=8000,4000&offset=0,0&autorotate=1&displaysize=800,500&fullsize=8000,4000&croppedsize=8000,4000&offset=0,0&autorotate=1" marginwidth="0" marginheight="0" scrolling="no" frameborder="0" height="100%" width="100%"></iframe> -->
    

