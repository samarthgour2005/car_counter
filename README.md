
## 🚗 Vehicle Detection & Counting using YOLOv8 and SORT Tracker  
This project detects and counts moving vehicles 🚙🚌🏍️ in a video feed using **YOLOv8** 🤖 for object detection and the **SORT** (Simple Online and Realtime Tracking) algorithm for tracking. It supports ⚡ GPU acceleration via **PyTorch CUDA** when available.  
###( Video can't be uploaded due to size restrictions ,images are provided)
### ✨ Features  
- 🎯 Real-time object detection with YOLOv8 (`ultralytics` library)  
- 🔍 Vehicle tracking using SORT algorithm  
- 🚗🚚🚌🏍️ Counts cars, trucks, buses, and motorbikes crossing a defined counting line  
- 🎭 Mask-based region of interest to focus on specific detection areas  
- 🖼️ Custom overlay graphics using `cvzone` for better visualization  
- ⚡ CUDA GPU support for faster inference (falls back to CPU if unavailable)  

### 🛠️ Technologies Used  
- 🐍 Python  
- 🎥 OpenCV (`cv2`)  
- 🔢 NumPy  
- 🤖 YOLOv8 (`ultralytics`)  
- 📍 SORT Tracker  
- 🖼️ cvzone  
- ⚡ PyTorch (with CUDA)  

### ⚙️ How it Works  
1. 📥 Loads YOLOv8 model and moves it to GPU if available.  
2. 🎭 Applies a mask to limit detection to a specific region of the video.  
3. 🚗 Detects vehicles in the region using YOLOv8.  
4. 📍 Tracks detected objects across frames using SORT.  
5. 🔢 Counts a vehicle when it crosses a predefined line.  
6. 🖼️ Displays bounding boxes, IDs, and the total count on the video.  
