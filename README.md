# On-Device ML with Kotlin

Code for an On-Device ML with Kotlin series on running machine learning models on Android with [LiteRT](https://ai.google.dev/edge/litert) (formerly TensorFlow Lite), written in Kotlin.

Each post has a matching checkpoint in this repo, so you can follow along step by step.

## The series

| Part | Topic | Post | Code |
|---|---|---|---|
| 1 | What LiteRT is and why on-device ML matters | [Read](https://medium.com/kotlinkenya-android254/part-1-on-device-ml-with-kotlin-2c45f3ec3d5c) | |
| 2 | Running your first model: inputs, outputs and a live camera | Coming soon | [Notebook](notebooks/01_mobilenet_v2_to_tflite.ipynb) |
| 3 | Bring your own model: train, convert, optimize, ship | Coming soon | |
| 4 | What LiteRT-LM is | Coming soon | |
| 5 | Running an LLM fully on-device | Coming soon | |
| Bonus | LiteRT in Kotlin Multiplatform | Coming soon | |

## Notebooks

### MobileNet V2 to LiteRT

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Jeremy-Gitau/on-device-ml-kotlin/blob/main/notebooks/01_mobilenet_v2_to_tflite.ipynb)

Converts a pretrained MobileNet V2 image classifier from TensorFlow 2 into a `.tflite` file, checks its input and output shapes, and tests it on a sample image before it goes into the Android app.

* **Input:** `[1, 224, 224, 3]` float32, pixels scaled to 0 to 1
* **Output:** `[1, 1001]` float32 logits (apply softmax for probabilities)

## License

Apache 2.0
