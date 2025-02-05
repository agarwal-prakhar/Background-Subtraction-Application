# Background Subtraction Application

This project demonstrates real-time **background subtraction** using the **mean frame technique**. It captures video from a webcam, computes the mean of the last 50 frames to estimate the background, and extracts the foreground by comparing the current frame with the computed background. A trackbar is provided to dynamically adjust the threshold for foreground detection.

![SBA2](https://github.com/user-attachments/assets/a8f4cfca-dfdb-489e-afb5-31640e689e51)


![SBA 6](https://github.com/user-attachments/assets/3c7a0ee4-524f-47b6-ab65-fe74b9e43c71)



## Features
- Real-time background subtraction using a webcam feed.
- Dynamic threshold adjustment using a trackbar.
- Efficient handling of frames using a rolling buffer (last 50 frames).
- Visualization of the original frame, computed background, and extracted foreground.

## Technologies Used
- **Python**: Core programming language.
- **OpenCV**: For video capture, image processing, and visualization.
- **NumPy**: For efficient array operations and mean computation.

## Installation and Setup in VS Code

Follow these steps to set up and run the project in **VS Code**:

### 1. **Clone the Repository**
   Open a terminal in VS Code and run the following command to clone the repository:

   ```bash
   git clone https://github.com/agarwal-prakhar/Background-Subtraction-Application.git
   cd Background-Subtraction-Application
```

## 2. Set Up a Virtual Environment
Create and activate a virtual environment to manage dependencies:

### On macOS/Linux:
```bash
python3 -m venv venv
source venv/bin/activate
```

### On Windows:
```bash
python -m venv venv
venv\Scripts\activate
```

## 3. Install Dependencies
Install the required Python packages using pip:

```bash
pip install -r requirements.txt
```


## 4. Run the Application
Open the script `Gausian_Mixture_Model.py` , `Frame_Differencing.py` ,and others in VS Code and run it:

- Click the **Run** button in the top-right corner of VS Code.
- Alternatively, use the terminal to run the script:

```bash
python Gausian_Mixture_Model.py
python Frame_Differencing.py
```

## 5. Use the Application
- A window will open showing the live video feed, computed background, and extracted foreground.
- Use the trackbar to adjust the threshold for foreground detection.
- Press the **q** key to exit the application.

## Troubleshooting
### Webcam Not Detected
- Ensure your webcam is connected and accessible. Test it using other applications like Zoom or your system's camera app.

### Dependency Issues
- Make sure all dependencies are installed correctly. If you encounter issues, try reinstalling them:

```bash
pip install --upgrade opencv-python numpy
```

### Inconsistent Indentation
- If you encounter indentation errors, ensure your editor is configured to use **4 spaces** for indentation (not tabs).

