# Coffee-Mug-Tracker

# ☕ Coffee Cup Detection & Tracking

This project demonstrates a simple solution for detecting and tracking coffee mugs in a video using a pre-trained YOLOv5 model and OpenCV's CSRT tracker. It is developed and tested entirely in Google Colab.

---

## 📌 Features

- Detects up to 2 coffee mugs using YOLOv5s model.
- Initializes CSRT trackers to track mugs across frames.
- Saves the output with bounding boxes and mug IDs.
- Demonstrates video processing in Python using OpenCV and Ultralytics YOLO.

---

## 🧩 Requirements

Install the following Python packages:

```bash
pip install ultralytics opencv-python-headless
```

---

## 🎞️ Input Video

Place your input video (e.g., `coffee_mugs.mp4`) in a suitable path like:

```plaintext
/content/drive/MyDrive/dataset/coffee_mugs.mp4
```

Output will be saved to:

```plaintext
/content/drive/MyDrive/dataset/mug_tracking_output.mp4
```

---

## 🚀 How to Run

Open the notebook in Google Colab or run the converted Python script. The notebook:

1. Mounts Google Drive to access the dataset.
2. Loads a pre-trained YOLOv5 model (`yolov5s.pt`).
3. Reads the input video and detects `cup` objects in the first frame.
4. Tracks those objects using OpenCV’s CSRT tracker in subsequent frames.
5. Draws bounding boxes and Mug IDs on each frame.
6. Saves the annotated video.

---

## 📂 Files in This Project

| File/Folder                          | Description                                      |
|-------------------------------------|--------------------------------------------------|
| `coffee_cup_detection_&_tracking.ipynb` | Main Jupyter Notebook containing the logic      |
| `README.md`                         | You’re here!                                     |
| `coffee_mugs.mp4`              | Sample input video    |
| `mug_tracking_output.mp4`           | Output video with tracking      |

---

## 🧪 Test Data Access

If you are not using your own video:
- Use from [Coffee Mug]([https://colab.research.google.com/drive/1FbaAyfhxhLkM3sHtlU76gP6RZKeBVRn8](https://www.pexels.com/video/video-of-men-talking-over-coffee-4667486/)).
- Or replace it with your own video containing mugs or cups.

---

## ✅ Evaluation

- The solution correctly detects and tracks mugs in the video.
- Works well when mugs are visible and not occluded.
- Tracks up to two mugs as designed.

---

## 📄 License

This project is open-source for academic and demonstration use.
