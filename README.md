# Face-mask detection coursework archive

Historical team coursework comparing YOLO and SSD experiments for face-mask detection. Start with [face-mask-detection](https://github.com/menesdeniz1/face-mask-detection) for the main portfolio version. This overlapping repository stays archived to preserve the coursework without presenting it as a separate flagship project.

## Report and experiment artifacts

- [Original project report](CMP3011_PROJECT_REPORT.docx), retaining the three contributors' attribution.
- [Result graphs](result_graphs/) and [SSD training plot](ssd_based_training_graph.png).
- `best.pt` and `ssd_face_mask_detector.pth`: historical model checkpoints.
- The original training notebooks, with the publication cleanup retained.

These are original coursework artifacts restored from the owner's backup in September 2026, not newly measured results. The report is retained unchanged as historical documentation: its description of SSD as TensorFlow-based does not match the PyTorch/torchvision implementation in the notebook. Treat the code as authoritative for implementation details. The reported comparisons have not been independently reproduced in this maintenance pass.

The report identifies a Kaggle Face Mask Detection dataset. Dataset redistribution and model/framework licensing are separate from owning the coursework: no new blanket license is granted over third-party inputs or pretrained components. Check the upstream terms before reuse. The raw training images are not included here.

## Running the camera example

Install `ultralytics` and `opencv-python` in an isolated environment. Set `MASK_MODEL_PATH` to a trusted compatible local YOLO checkpoint, then run `python webcamtest.py` only when camera access is intended. The entry point does not download a model automatically. Notebook paths and dependencies reflect the original training environment and may require adaptation.

Only load model checkpoints you trust; serialized model files may execute code when deserialized. The restored files have not been loaded or retrained during maintenance.

## Archive scope

The report, plots and weights were restored in a new commit without reverting the source/privacy repairs or restoring old commit history. The original webcam video was not copied back because permission to publish every identifiable person was not established. A demo can be added separately with that permission or after anonymization.
