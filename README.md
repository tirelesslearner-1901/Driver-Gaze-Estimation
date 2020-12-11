# Driver-Gaze-Estimation
Driver Gaze estimation using Convolutional Neural Networks  
# Datasets
## LISA Gaze Dataset v0
Download the complete RGB dataset for driver gaze classification using this [link](https://drive.google.com/file/d/1Ez-pHW0v-5bRdz8NjTLlzWZPT0GS2rYT/view).
### Training (v0 RGB data)
The SqueezeNet gaze classifier can be trained using the following command:
python gazenet.py --dataset-root-path=/path/to/lisat_gaze_data_v0/ --version=1_1 --snapshot=./weights/squeezenet1_1_imagenet.pth --random-transforms
### Inference (v0 RGB data)
Inference can be carried out using the command as follows:
python infer.py --dataset-root-path=/path/to/lisat_gaze_data_v0/ --split=val --version=1_1 --snapshot-dir=/path/to/trained/rgb-model/directory/ --save-viz

## LISA Gaze Dataset v1
Download the complete RGB dataset for driver gaze classification using this link.
### Training (v1 RGB data)
The SqueezeNet gaze classifier can be trained using the following command:
python gazenet.py --dataset-root-path=/path/to/lisat_gaze_data_v1/ --version=1_1 --snapshot=./weights/squeezenet1_1_imagenet.pth --random-transforms
### Inference (v1 RGB data)
Inference can be carried out using the command as follows:
python infer.py --dataset-root-path=/path/to/lisat_gaze_data_v1/ --split=val --version=1_1 --snapshot-dir=/path/to/trained/rgb-model/directory/ --save-viz



