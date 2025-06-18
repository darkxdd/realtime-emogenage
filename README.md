# Face Age Gender Flask Code

This project is a Flask application for detecting face, age, and gender from images.

## Setup and Installation

Follow these steps to set up and run the project locally:

### 1. Clone the repository

```bash
git clone https://github.com/darkxdd/realtime-emogenage.git
cd realtime-emogenage
```

### 2. Create a virtual environment (recommended)

```bash
python -m venv .venv
```

### 3. Activate the virtual environment

**On Windows:**

```bash
.venv\Scripts\activate
```

**On macOS/Linux:**

```bash
source .venv/bin/activate
```

### 4. Install dependencies

Install the required Python packages using `pip`:

```bash
pip install -r requirements.txt
```

### 5. Run the Flask application

```bash
python run.py
```

### 6. Access the application

Open your web browser and navigate to `http://127.0.0.1:5000/` to access the application.

## Project Structure

- `age_model_50epochs.h5`: Pre-trained model for age detection.
- `emotion_detection_model_100epochs.h5`: Pre-trained model for emotion detection.
- `gender_model_50epochs.h5`: Pre-trained model for gender detection.
- `haarcascade_frontalface_default.xml`: Haar Cascade classifier for face detection.
- `face.py`: Contains the core logic for face, age, and gender detection.
- `run.py`: The main Flask application file.
- `requirements.txt`: Lists all Python dependencies.
- `static/`: Contains static files like images.
- `templates/`: Contains HTML templates for the web interface.

## Git LFS

This project uses Git LFS (Large File Storage) to manage large model files (`.h5`). Ensure you have Git LFS installed before cloning the repository to properly download these files.

To install Git LFS, follow the instructions on the official Git LFS website: <mcurl name="https://git-lfs.com/" url="https://git-lfs.com/"></mcurl>

After installation, you can verify it with:

```bash
git lfs install
```

And ensure `.h5` files are tracked:

```bash
git lfs track "*.h5"
```