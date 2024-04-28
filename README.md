## 👋 hello

This script performs traffic flow analysis using YOLOv8, an object-detection method and ByteTrack, a simple yet effective online multi-object tracking method. It uses the supervision package for multiple tasks such as tracking, annotations, etc.

[![Traffic Analysis Result](https://res.cloudinary.com/marcomontalbano/image/upload/v1714279684/video_to_markdown/images/google-drive--1qAjfZProh9qKc30b-uyJSnHXXVPefCpS-c05b58ac6eb4c4700831b2b3070cd403.jpg)](https://drive.google.com/file/d/1qAjfZProh9qKc30b-uyJSnHXXVPefCpS/view?usp=drive_link "Traffic Analysis Result") 


## 💻 install

- clone repository and navigate to example directory

    ```bash
    git clone https://github.com/roboflow/supervision.git
    cd supervision/examples/traffic_analysis
    ```

- setup python environment and activate it [optional]

    ```bash
    python3 -m venv venv
    source venv/bin/activate
    ```

- install required dependencies

    ```bash
    pip install -r requirements.txt
    ```

- download `traffic_analysis.pt` and `traffic_analysis.mov` files

    ```bash
    ./setup.sh
    ```

## ⚙️ run

```bash
python script.py \
--source_weights_path data/traffic_analysis.pt \
--source_video_path data/traffic_analysis.mov \
--confidence_threshold 0.3 \
--iou_threshold 0.5 \
--target_video_path data/traffic_analysis_result.mov
```
# Traffic-analysis-with-YOLOv8
