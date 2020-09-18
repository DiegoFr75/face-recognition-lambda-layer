# Lambda layer to use face recogniton on AWS Lambda (Python 3.6)

# Python dependencies
1. dlib==19.21.0
2. face_recognition
2. face-recognition-models==0.3.0
3. numpy==1.15.4
4. Pillow==7.2.0

# Creating a lambda layer
1. Download "face_recognition_layer.zip"
2. Upload to s3
3. Get the file url (ex: https://{bucket}.s3.amazonaws.com/dir/to/file.zip)
4. Go to, Lambda > Layers > Create Layer
5. Give an name to your layer
6. Select "Upload an Amazon S3 file" and insert the file url
7. Select Python 3.6 on "Supported execution times"
8. Click on "create" button

Now you just need to add this layer to your lambda function