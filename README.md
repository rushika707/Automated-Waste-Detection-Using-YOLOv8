# Automated-Waste-Detection-Using-YOLOv8
Object detection project using YOLOv8 to detect and classify waste items, trained and evaluated on the TACO dataset.

An AI-powered waste detection system using YOLOv8, trained and evaluated on the [TACO Dataset](http://tacodataset.org/).  
This project aims to automatically detect and classify waste items from images, helping with smart waste management and environmental sustainability.

---

## 📌 Features
- **Object Detection**: Detects multiple waste categories in an image.
- **YOLOv8 Model**: Leveraging Ultralytics' YOLOv8 for high accuracy.
- **Custom Training**: Trained on the TACO dataset for waste classification.
- **Evaluation Metrics**: mAP, Precision, Recall, and Confusion Matrix.

---

## 📂 Dataset
- **Name**: TACO (Trash Annotations in Context)
- **Description**: A dataset of waste images annotated for detection and segmentation.
- **Link**: [TACO Dataset](http://tacodataset.org/)

---

## 🚀 Installation
```bash
# Clone the repository
git clone https://github.com/rushika707/Automated-Waste-Detection-Using-YOLOv8.git
cd Automated-Waste-Detection-Using-YOLOv8

# Install dependencies
pip install -r requirements.txt
````

---

## 🏋️ Training

```bash
yolo task=detect mode=train data=taco.yaml model=yolov8n.pt epochs=50 imgsz=640
```

---

## 📊 Evaluation

```bash
yolo task=detect mode=val model=runs/detect/train/weights/best.pt data=taco.yaml
```

---

## 📸 Inference

```bash
yolo task=detect mode=predict model=runs/detect/train/weights/best.pt source=path/to/images
```


## 🤝 Contributing

Contributions are welcome! Feel free to fork this repo, create a feature branch, and submit a pull request.

---

## ✨ Author

**Rushika Sree**
📧 Email: rushikasree12@gmail.com

```
