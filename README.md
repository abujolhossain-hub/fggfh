# Video Merger Website - Render Ready

## Requirements

- Python 3.7+
- ffmpeg binary included in ./bin/ffmpeg (already included)
- Internet connection for installing python packages

## Setup Backend

1. Install dependencies:

```bash
pip install -r requirements.txt
```

2. Run backend server:

```bash
python app.py
```

Backend will run on the port specified by Render or default 5000.

## Setup Frontend

1. Open `index.html` in browser or host it on any static hosting.

2. Edit the backend URL in `index.html` JavaScript fetch call (`https://YOUR-RENDER-SERVICE.onrender.com/upload`) to your deployed backend URL.

## Notes

- ffmpeg binary is included for compatibility with Render.
- Temporary upload and merged files are stored in `/tmp` folder as Render filesystem is ephemeral.
- CORS is enabled in backend.
