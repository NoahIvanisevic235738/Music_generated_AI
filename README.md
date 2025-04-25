# Music_generated_AI

## Project Description
This project explores AI-powered music generation using various models and techniques. Currently, it features implementation of Facebook's MusicGen model through HuggingFace Transformers.

## Repository Structure
```
Music_generated_AI/
├── Deliverables/
│   └── MusicGen (HuggingFace Transformers).ipynb
└── README.md
```

## Features
- Text-to-music generation using MusicGen
- Support for both CPU and GPU processing
- WAV file output format
- Customizable text prompts for music generation

## Requirements
- Python 3.x
- PyTorch
- Transformers library
- SciPy
- CUDA-compatible GPU (optional but recommended)

## Installation
```bash
pip install torch transformers scipy
```

## Usage
1. Open the Jupyter notebook in the Deliverables folder
2. Run all cells in the notebook
3. The model will generate music based on the provided text prompt
4. Output will be saved as 'musicgen_output_large.wav'

### Example Prompt
```python
"A gentle classical piano solo, which sounds sad and melancholic"
```

## Technical Details
- Model: facebook/musicgen-large
- Output format: WAV
- Sampling rate: Model default (determined by configuration)
- Generation length: Controlled by max_new_tokens parameter

## Limitations
- Large model requires significant GPU memory
- Generation process can be time-consuming
- Output length is constrained by model architecture

## Contributing
Feel free to open issues or submit pull requests for improvements.

## Acknowledgments
- Facebook Research for the MusicGen model
- HuggingFace for the Transformers library