# Model-performance-Estimator

Our deep learning based document image processing solution utilizes advanced algorithms to enhance the text and overall resoltion of scanned documents. This solution can improve the quality and readability of document images captured inaccurately and also enhance the performance of optical character recognition (OCR) systems. This solution helps improve performance of various down stream activities performed on documents. This solution takes a zip file of low resolution document image/images as input and returns a zip file of transformed image/images as output. This solution supports jpg and png file formats. Limit the number of images to around 20 for optimal use on low end machines.

## Amazon SageMaker



### Input :

A zip file with low resolution document images is required as input. Please refer sample images


### Output:



Content type: application/zip



### Invoking endpoint



AWS CLI Command
If you are using real time inferencing, please create the endpoint first and then use the following command to invoke it:



`aws sagemaker-runtime invoke-endpoint --endpoint-name "endpoint-name" --body fileb://input.zip --content-type application/zip --accept application/zip responce.zip`



**Substitute the following parameters:**



* "endpoint-name" - name of the inference endpoint where the model is deployed
* input.zip - input file
* application/zip - MIME type of the given input file (above)
* responce.zip - filename where the inference results are written to.
