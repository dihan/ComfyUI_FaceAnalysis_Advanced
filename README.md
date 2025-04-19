# Face Analysis for ComfyUI (Advanced Fork)

This is an advanced fork of [ComfyUI_FaceAnalysis](https://github.com/cubiq/ComfyUI_FaceAnalysis) that adds additional face analysis capabilities through InsightFace. This fork extends the original functionality with:

- Age estimation
- Gender recognition (enhanced)
- Expression analysis
- Gaze detection
- Anti-spoofing detection
- 3D face reconstruction

These features are available directly through the InsightFace class without requiring additional nodes, making it easier to integrate advanced face analysis into your workflows.

## Why This Fork?

The original ComfyUI_FaceAnalysis is a great tool for basic face analysis, but InsightFace offers many more capabilities that weren't exposed in the original implementation. This fork aims to make these advanced features easily accessible while maintaining compatibility with the original codebase.

> [!IMPORTANT]  
> **2025.04.14** - I do not use ComfyUI as my main way to interact with Gen AI anymore as a result I'm setting the repository in "maintenance only" mode. If there are crucial updates or PRs I might still consider merging them but I do not plan any consistent work on this repo.

## Installation

You need to install either InsightFace or Dlib (or both).

For DLIB download [Shape Predictor](https://huggingface.co/matt3ounstable/dlib_predictor_recognition/resolve/main/shape_predictor_68_face_landmarks.dat?download=true), [Face Predictor 5 landmarks](https://huggingface.co/matt3ounstable/dlib_predictor_recognition/resolve/main/shape_predictor_5_face_landmarks.dat?download=true), [Face Predictor 81 landmarks](https://huggingface.co/matt3ounstable/dlib_predictor_recognition/resolve/main/shape_predictor_81_face_landmarks.dat?download=true) and the [Face Recognition](https://huggingface.co/matt3ounstable/dlib_predictor_recognition/resolve/main/dlib_face_recognition_resnet_model_v1.dat?download=true) models and place them into the `dlib` directory.

Precompiled Dlib for Windows can be found [here](https://github.com/z-mahmud22/Dlib_Windows_Python3.x).

![face analysis](./face_analysis.jpg)

The extension also supports [AuraFace](https://huggingface.co/fal/AuraFace-v1/tree/main) that is a free alternative to InsightFace. Download all the files and place them under `models/insightface/models/auraface/`
