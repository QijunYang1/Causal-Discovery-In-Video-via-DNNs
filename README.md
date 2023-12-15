
### [our real google drive](https://drive.google.com/drive/folders/1zSfbF2Nk4oLh6U5NoPAc0LnLpip3G1eV?usp=sharing)

### Group Members
- Horan Liu
	- NetID: hl449
- Elinor Cheng
	- NetID: yc493
- Qijun Yang
	- NetID: qy37
	
	
# Repository Structure

- `Final_Report_Causal_Discovery_In_Video_via_DNNs.pdf`: Final report

- FasterRCNN_NGC
    - Players_central_points
        - `cxcy.pkl`: Predicted labels (cx, cy) by Faster RCNN for the video data v_-6Os86HzwCs_c009.
    - FasterRCNN_checkpoint
        - `checkpoint4`: Checkpoint data of Faster RCNN trained for 5 epochs.
    - `FasterRCNNwithNeuralCausality.ipynb`
        - This Jupyter notebook includes the complete workflow:
            - Data preprocessing
            - Training the Faster RCNN model
            - Training the Neural Causality Network
            - Visualize Object Location Time Series
            - Generating the Granger Causality Matrix

- Yolo_deepsort_NGC
    - Models: Granger Causality Models
        - `clstm.py`
        - `cmlp.py`
        - `crnn.py`
    - `synthetic.py`: generate sample lorenz series
    - `yolodeepsort.zip`: the code for deepsort
    - `NGC.ipynb`: granger causality for sample lorenz and objects bound boxes
    - `yolotrack.ipynb`: track based on yolo using yolodeepsort.zip

- YOLOv8_NGC
    - Models: Granger Causality Models
        - `clstm.py`
        - `cmlp.py`
        - `crnn.py`
    - Data and saved model:
        - data for yolo:training data for yolo
            - `data.zip`
                - cutom
                    - images:training images
                    - labels: training labels
                    - `train.txt`: train set
                    - `test.txt`: test set
                    - `val.txt`: validation set
            - `data.yaml`
                    - parameters for YOLOv8 training
        - YOLOv8_weights
            - `best.pt`:trained with un-mask pictures
            - `best_blur.pt`:trained with randomly blurred pictures
            - `best_mask.pt`:trained with randomly masked pictures
    - `yolo_data.ipynb`:
        - Transform data into centerpoints format
        - Data normalization
        - Split the dataset
    - `yolov8.ipynb`: YOLOv8 training 
        - Train with unmasked pictures
        - Randomly mask/blur the pictures
        - Train with randomly masked/blurred pictures
    - `NGC-cMLP.ipynb`:
        - Detect randomly masked pictures with pre-trained YOLOv8
        - Visualize the predicted coordinates series
        - Train the cMLP model with predicted label and true label
        - Visualize and compare the GC matrix
    
- SportsMOT_example
    - dataset
        - train
            - xxx(dataset name from splits_txt)
                - `gt`: ground true box.txt
                - img1: sequence of images.jpg
    - `splits_txt`: 
        - ource:https://paperswithcode.com/dataset/sportsmot
