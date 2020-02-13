# Object-Detection-Confusion-Matrix
Directly Calculate the object detection confusion matrix from tfrecords.


To run the code 

    python code.py data/test.record model/frozen_inference_graph.pb model/label_football.pbtxt confusion_matrix.csv
    
where 

    input_tfrecord_paths=sys.argv[1] #'A comma separated list of paths to input TFRecords.'
    inference_graph=sys.argv[2] #'Path to the inference graph with embedded weights.'
    label_map=sys.argv[3] # 'Path to the label map'
    output_path=sys.argv[4]#'Path to the output the results in a csv.'





##### Resources:
The code is taken from https://github.com/svpino/tf_object_detection_cm, only tensorflow object detection api Dependency files are placed to work it autonomously. 
