# windows conda
conda create --name basketball python=3.10
pip install torch==2.4.1 torchvision==0.19.1 torchaudio==2.4.1 --index-url https://download.pytorch.org/whl/cu124
pip install flask flask_socketio opencv-python ultralytics eventlet

# jetson conda
conda create --name basketball python=3.10
## https://forums.developer.nvidia.com/t/pytorch-for-jetson/72048
## jetpack6 + CUDA12.4
pip install torch-2.3.0xxx
pip install torchvision-0.18.0xxx
pip install opencv-python ultralytics
pip install numpy==1.26.4
pip install flask flask_socketio opencv-python ultralytics eventlet


# fyp 1
frontend
npm install
npm run start

backend
pip install cvzone reportlab flask_cors 

# fyp 2
frontend
npm install
npm run dev
http://localhost:5173/live/v4

backend
pip install fastapi av aiortc uvicorn scikit-learn   
uvicorn main:app --reload --host 0.0.0.0 --port 8000
