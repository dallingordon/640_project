# 640_project
640_project

<h2>Images Folder</h2>
This is where the images are stored.  /Imgaes/PreRequest contains the images before the edits.  /Images/PostRequest are results (targets).
<h3>PreRequest</h3>
    These are the input images.  Following the link in the Images.csv will display this image for each request. These were the images fed to both stable diffusion and Dall-e 2 to generate the images in those folders.
<h3>Post Request</h3>
    These are the human photoshopped images.  We selected them from the comments of the reddit posts.  We tried to select the image that we deemed the most accurate to the request. 
<h3>SD_out</h3>
    These are the images resulting from passing the prompt and the PreRequest image into stable diffusion.
<h3>Dalle2_out</h3>
    These images are the PreRequest images that were passed through Dalle-2.  These images requeired a user generated mask.  We did these using our best judgement based on the image and the request text.  We selected the image that was the most representative of the Dall-e 2 results. If the results were consistently good, we chose a good image.  If there was a salient error throughout the Dall-e 2 results for a given input image and request, we tried to select the image best portrayed the behavior of the model.
<h3>Images.csv</h3>
    This file contains data on each image with the following headers:</br></br>
<i>id</i></t> unique identifier</br>
<i>pre_request_file_name</i></t> File name for the pre-request. (input) image</br>
<i>post_request_file_name</i></t> Human generated photoshopped image.</br>
<i>sd_file_name</i></t> Stable diffusion result.</br>
<i>dalle_2_name</i></t> Dall-e 2 result.</br>
<i>request_text</i></t> The request provided from reddit titles.  We did some cleaning to make it more concise.</br>
<i>reverse_request</i></t> This is a data augmentation opportunity that we will look into in later steps.  Our thinking is that we can swap the photoshopped and the input images to generate the opposite request.</br>
<i>link</i></t> Link the the reddit image source.</br>
<i>watermark</i></t> If a watermark is present.</br>
<i>difficulty_</i></t> A column for each group member to asses the request difficulty.</br>

<h2>Image_Comparison.ipynb</h2>
Images and requests displayed.
