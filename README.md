# Audio CAPTCHA Generator

A Python-based project to generate and play audio CAPTCHAs. This project is useful for enhancing accessibility and security by providing audio-based CAPTCHA solutions.

## Features

- Generate random text-based CAPTCHAs.
- Convert CAPTCHA text to audio using Google Text-to-Speech (gTTS).
- Play the audio CAPTCHA directly using the PyDub library.

## Requirements

- Python 3.7 or higher
- Libraries:
  - `pyttsx3`
  - `pydub`
  - `gtts`

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/thekartikeyamishra/AudioCAPTCHAGenerator.git
   cd AudioCAPTCHAGenerator
   ```

2. Install the required dependencies:
   ```bash
   pip install pyttsx3 pydub gtts
   ```

3. Ensure you have the required system dependencies for `pydub`:
   - Install FFmpeg: 
     - On Ubuntu/Debian:
       ```bash
       sudo apt-get install ffmpeg
       ```
     - On Windows, download FFmpeg from [FFmpeg website](https://ffmpeg.org/download.html) and add it to your system's PATH.

## Usage

1. Run the script:
   ```bash
   python audio_captcha_generator.py
   ```

2. The script will:
   - Generate a random CAPTCHA.
   - Save the CAPTCHA audio as an MP3 file.
   - Play the audio CAPTCHA using PyDub.

3. Example output:
   ```bash
   Generated CAPTCHA: AB12CD
   Audio CAPTCHA saved as audio_captcha.mp3
   ```

## Code Explanation

1. **Generate Random CAPTCHA**:
   The `generate_random_captcha` function creates a random string of uppercase letters and digits with a default length of 6.

2. **Convert CAPTCHA to Audio**:
   The `generate_audio_captcha` function uses the `gTTS` library to convert the CAPTCHA text into an MP3 audio file.

3. **Play Audio CAPTCHA**:
   The `play_audio_captcha` function uses the `PyDub` library to play the generated audio file.


## Contact

For questions or feedback, please contact:

- **Author**: Kartikeya Mishra
- **Email**: workmailkartikeya@gmail.com
- **GitHub**: [thekartikeyamishra](https://github.com/thekartikeyamishra)

