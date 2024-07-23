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
python3 classify.py --model 
```

*   You can optionally specify the `model` parameter to set the TensorFlow Lite
    model to be used:
    *   The default value is `movinet_a0_int8.tflite`
    *   This sample currently uses MoviNet-A0, but it supports all TensorFlow
        Lite
        [MoviNet video classification](https://tfhub.dev/s?deployment-format=lite&q=movinet)
        models that are available on TensorFlow Hub. You can use the larger
        variant of MoviNet if you need higher accuracy.
*   You can optionally specify the `maxResults` parameter to limit the list of
    classification results:
    *   Supported value: A positive integer.
    *   Default value: `3`.
*   Example usage: `python3 classify.py \ --model movinet_a0_int8.tflite \
    --maxResults 5`

For more information about executing inferences with TensorFlow Lite, read
[TensorFlow Lite inference](https://www.tensorflow.org/lite/guide/inference).
