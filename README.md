<h1>Cat and Dog picture classification:</h1>
Data : https://www.kaggle.com/datasets/salader/dogs-vs-cats
 <h1> Kegal Work </h1>
 1. First open the path mentioned up
 2. Go to profile and then go to account then scroll down to create token under API
 3. Create it and upload it over driver
 4. run 
   ! mkdir -p ~/.kaggle
   ! cp kaggle.json ~/.kaggle/
   code 
5. paste the API key and run it by this the data from kegal will fetch to G driver in zip folder
6. <h4>unzip the folder with below code</h4>
    import zipfile
    zip_ref = zipfile.ZipFile('dogs-vs-cats.zip', 'r')
    zip_ref.extractall('/content')
    zip_ref.close()


<H1>Conver images to 256, 256 pxl </H1>
-Converted both train and test data set those were provided by keggal
- Normalized all of them to 1 and 0 by deviding by 256

<h1>CNN Model</h1>
-- Created 6 layered model 3 were convuluted and 3 ann with batch normalization and dropout 
-- used padding valid and filter size 3,3 for and used max pooling with 2,2 shape

<h1>Result gave 83% accuracy with Test Data</h1>

 
