# Phonemesh voice packs

Speech files for the Phonemesh Android app. The app downloads them once, checks each file against a hash built into the app, and then works without internet. The files are attached to this repository's releases; there is no code here.

| File | What it is | Made from | Licence of the original |
|---|---|---|---|
| `phonemesh-engine-whisper-tiny-1.zip` | Speech to text, small | OpenAI Whisper tiny, ONNX conversion from [sherpa-onnx](https://github.com/k2-fsa/sherpa-onnx/releases/tag/asr-models) | MIT |
| `phonemesh-engine-whisper-base-1.zip` | Speech to text, larger | OpenAI Whisper base, ONNX conversion from [sherpa-onnx](https://huggingface.co/csukuangfj/sherpa-onnx-whisper-base) | MIT |
| `phonemesh-voice-fr-siwis-1.zip` | French voice | Piper voice `fr_FR-siwis-low` ([model card](https://huggingface.co/rhasspy/piper-voices/blob/main/fr/fr_FR/siwis/low/MODEL_CARD)), trained on the [SIWIS French Speech Synthesis Database](https://datashare.is.ed.ac.uk/handle/10283/2353); packaged by [sherpa-onnx](https://github.com/k2-fsa/sherpa-onnx/releases/tag/tts-models) | CC BY 4.0 |
| `phonemesh-voice-en-US-ljspeech-1.zip` | English voice | Piper voice `en_US-ljspeech-medium` ([model card](https://huggingface.co/rhasspy/piper-voices/blob/main/en/en_US/ljspeech/medium/MODEL_CARD)), trained on the [LJ Speech Dataset](https://keithito.com/LJ-Speech-Dataset/); packaged by sherpa-onnx | Public domain |

Both voices include pronunciation data from [espeak-ng](https://github.com/espeak-ng/espeak-ng), licensed GPL-3.0.

Each ZIP holds a `NOTICE.txt` with these attributions, a `SOURCES.json` naming the exact upstream file and its SHA-256, and a `SHA256SUMS` of its contents. The models are unchanged from the upstream files apart from repackaging.

## SHA-256

```
f2d7a07582cc96b068a94a2b53956107586bca0e5cc45efb7cce093b2b2e70ad  phonemesh-engine-whisper-tiny-1.zip
75de028225062e404daaad428b78ac7f27d815895ce0ed3754c1a326b9e74460  phonemesh-engine-whisper-base-1.zip
d07335772d3f9beb9ba1d7d5da75b347d26976d576feaf4be79a89f5f182c9a8  phonemesh-voice-fr-siwis-1.zip
ef6026904f8f1fa3ffa2c6373f9f5857117ffa43d4d3ecb22d59c8b2d7eda1cc  phonemesh-voice-en-US-ljspeech-1.zip
```
