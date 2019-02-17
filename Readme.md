With this repository I introduce a unique and rich dataset based on the original **MSCOCO image captionaing dataset**.
<br />
<br />
Find sample json files containing:
<br />
1. Name of image from MSCOCO
2. Number of objects present in the image
3. Class label of the object
4. 100-dimensional word embedding vector based on Word2Vec for the class label
5. 4096-dimensional object embedding vector for each instance of the object(based on AlexNet)
6. Bounding box information for each object instance
7. Distance of each object instance from the origin(top-left) of the image
<br />
<br />
Format of the dataset:
<br />
The dataset is split into multiple JSON files. Each JSON file contains a list of dictionaries where each dictionary is pertaining to a single image from the MSCOCO image captioning dataset.
<br />
[{<name of image>:{'num_objects':<number of objects>, 'objects': [{'object_lable':<name of object>, 'object_word_embedding':<word2vec based object label features>, 'feature_vectors':[{'object_visual_embedding':<alexnet based object visual features>}&ast], 'bounding_box':<x,y position of the object>, 'distance': <object distance from top-left position inside image>}&ast]}}&ast]
<br />
<br />
&ast - items are repeatable
<br />
<br />
Find attached with this repository sample JSON files from this dataset inside the **sample** folder.

&astNote&ast: If you are interested in playing around with this dataset and need to have access to the full dataset, feel free to contact me through ![](ashutosh.mishra1014@gmail.com)