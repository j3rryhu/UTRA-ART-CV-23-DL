## Models
All models are based on Yolov8n and trained under the same dataset (photos captured in the competition track video with some augmentation applied)
- Train9: 20 epochs
- Train15: 50 epochs
- Train16: 30 epochs

All models are able to detect potholes with occasional false positives. Train16 has the best performance with fewest instances of false positive.
Note: Inference time with OpenVino and ONNX models only improve under CPU inference.

## Inference time
Tested on 10 jpg photos consecutively where each photo has size ~650KB (train9)
- GTX 1070: 8.3ms
- GTX 1080: 8.7ms
- RTX 2070: 5.2ms
- RTX 4090: 1.7ms
