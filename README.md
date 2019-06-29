# jackAudio
 A Python package for stationary audio noise reduction.

Details: [J.A.C.K.](https://github.com/cooperbarth/Joint-Audio-Correction-Kit)

## Usage
`python3 -m pip install jackAudio`

```python
import librosa
from jackAudio import filterAudio

READ_PATH = "./my_audio.wav"
AUDIO_SR = 44_100
WRITE_PATH = "./clean_audio.wav"

audio, sr = librosa.load(READ_PATH)
_ = filterAudio(audio, sr, WRITE_PATH)
```
