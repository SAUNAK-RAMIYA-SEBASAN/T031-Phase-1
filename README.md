<div align="center">

# 💵 Smart Currency Detection & Transaction Verification

### Phase 1 — Currency Detection & Wearable Integration

<p align="center">
  <a href="T031_ProjectReport.pdf">
    <img src="https://img.shields.io/badge/Deliverable-Project%20Report-FF6B35"/>
  </a>
  <a href="T031_Paper.pdf">
    <img src="https://img.shields.io/badge/Deliverable-Conference%20%2F%20Journal%20Paper-4A90D9"/>
  </a>
  <a href="T031_DemoVideo.mp4">
    <img src="https://img.shields.io/badge/Deliverable-Demo%20Video-E94560"/>
  </a>
  <img src="https://img.shields.io/badge/Team-T031-10B981"/>
  <img src="https://img.shields.io/badge/Detector-YOLOv8n-FFD166?style=flat-square"/>
  <img src="https://img.shields.io/badge/Edge%20Runtime-ONNX%20%2F%20TFLite-2D9CDB?style=flat-square"/>
  <img src="https://img.shields.io/badge/Voice-Piper%20TTS-8E44AD?style=flat-square"/>
</p>

</div>

---

## About

Phase 1 delivers the real-time currency detection core: a YOLOv8n model trained to
identify currency notes from a live camera feed, exported to an edge-friendly format
and paired with a text-to-speech layer that speaks the detected denomination aloud
for hands-free use on a wearable device.

## Phase 1 — Completed

- [x] **Dataset prep** — `data.yaml` paths fixed, class mappings verified, train/valid splits confirmed
- [x] **YOLOv8n training** — Model trained on the dataset; precision, recall, mAP@0.5 and inference latency logged
- [x] **Model export** — Trained weights converted to ONNX / TFLite for on-device inference
- [x] **Detection module** — `src/detection/` built: model loading, inference, post-processing (class + confidence)
- [x] **Config tuning** — `src/config/settings.py` populated with thresholds taken from the training results
- [x] **Audio module** — `src/audio/` built: Piper TTS speaks the detected currency aloud

## Tech Stack

| Layer | Technology |
| --- | --- |
| Language | Python |
| Detection | YOLOv8n (Ultralytics) |
| Edge export | ONNX / TFLite |
| Speech | Piper TTS |

## File Structure

```
Project-Phase-1/
├── README.md
├── T031_ProjectReport.pdf     # Soft copy project report
├── T031_Paper.pdf             # Submitted conference / journal paper
└── T031_DemoVideo.mp4         # Full video demonstrating each module
```

<div align="center">

**Team T031**

</div>
