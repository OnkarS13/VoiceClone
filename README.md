## Environment Setup

Please follow these instructions in a Python environment greater than 3.8:

### Windows/Linux:
1. Install essential dependencies using pip:
   ```bash
   pip install torch torchvision torchaudio
macOS:
Install essential dependencies using pip:
bash
Copy code
pip install torch torchvision torchaudio
Additional Pretrained Models and Data
RVC requires additional pretrained models and data for inference and training. You can download these models from our Hugging Face space.

Here is a list of the required pretrained models and other files:

./assets/hubert/hubert_base.pt
./assets/pretrained
./assets/uvr5_weights
If you want to test the v2 version of the models, you'll also need:

./assets/pretrained_v2
For Windows users, you may need ffmpeg.exe and ffprobe.exe. Ubuntu/Debian users can install these using apt install ffmpeg, and Mac users can use brew install ffmpeg.

If you want to use the latest RMVPE pitch extraction algorithm, you'll need to download the pitch extraction model parameters and place them in the RVC root directory: rmvpe.pt

For Nvidia and AMD GPU users, you'll need the DML environment. Download rmvpe.onnx.
Running the WebUI
To start the WebUI, use the following command:

bash
Copy code
python infer-web.py
For Windows and macOS users, you can download and unzip RVC-beta.7z. Windows users can run go-web.bat to start the WebUI, and macOS users can run sh ./run.sh.
