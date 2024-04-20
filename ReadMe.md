## Speech Processing

This repository contains code for various speech processing tasks.

**Subfolders:**

* **speech_preprocessing:**  Contains functions for preprocessing speech audio, including:
    * Spectrogram calculation
    * Noise cancellation (using spectral subtraction)
* **wavs:** Stores audio files used in the examples.

**Files:**

* **Noise_cancelling.py:** Implements functions for calculating spectrograms, noise cancellation, and audio reconstruction.
* **speech_segmentation.py:** Implements a basic speech segmentation engine using energy-based detection.

**Noise Cancellation**

The `Noise_cancelling.py` file provides functions for:

* Spectrogram calculation (`spectrogram` and `spectrogram2wav`) for converting between time and frequency domains.
* Noise cancellation (`NoiseCancelling`) using spectral subtraction to remove noise from an audio signal.

**Speech Segmentation**

The `speech_segmentation.py` file demonstrates a simple speech segmentation engine based on energy levels. The `Engine` class implements methods for:

* Calculating energy of the audio signal.
* Updating a dynamic threshold based on background noise.
* Detecting speech segments based on energy exceeding the threshold for a minimum duration.

**Running the Examples**

This repository requires libraries like `numpy`, `matplotlib.pyplot`, `scipy.io.wavfile`, and `IPython.display` (for audio playback). Make sure you have them installed before running the scripts.

The provided code snippets showcase the functionalities. You can modify them to suit your specific needs.

**Future Work**

This repository serves as a starting point for speech processing tasks. Here are some potential areas for future development:

* Implementing more sophisticated noise cancellation techniques.
* Utilizing feature extraction methods for speaker recognition or speech classification.
* Refining the speech segmentation engine for better accuracy.

Feel free to explore, modify, and contribute to this repository!
