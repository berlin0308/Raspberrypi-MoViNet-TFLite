#  Running MoViNet-Stream Models on Raspberry Pi with TFLite


## 1. Download Code Example

```
git clone https://github.com/berlin0308/raspberrypi-tflite-movinet --depth 1
```

## 2. Install Python Packages

```
sh setup.sh
```

## 3. Run Inference

```
python3 classify.py --model models/a1_v2_stream_b16_lr0.0001_g1.5_d0.5_92/a1_float16.tflite
```

+ ```--model``` : MoViNet model path
+ ```--label``` : Path to the label map txt
+ ```--numThreads``` : CPU threads to run the model
