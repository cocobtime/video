# Video Generator with Text-to-Speech

This project generates videos with audio from comments, using the gTTS library for text-to-speech and moviepy for video editing.

## Files

- `gtts_gen.py`: Main script for generating videos with audio from comments.
- `combine_media.py`: A script for combining media files.
- `character.json`: JSON file containing character data (name, video link).
- `comment.json`: JSON file containing post and comment data.
- `config.json`: JSON file containing configuration settings for the video generation.
- `audio_outputs/`: Directory where generated audio files are stored.
- `video_outputs/`: Directory where generated video files are stored.
- `base/`: Directory containing base GIF files.
- `xaudio/`: Directory containing example audio and video files.
- `coqui_env/`: Python virtual environment for coqui-ai.
- `venv39/`: Python virtual environment.

## How to Use

1.  Make sure you have Python 3.6 or higher installed.
2.  Install the required libraries:
    ```bash
    pip install gTTS moviepy
    ```
3.  Create `character.json` and `comment.json` files with the appropriate data.
4.  Run the `gtts_gen.py` script with the post ID you want to process:
    ```bash
    python gtts_gen.py --post_id <post_id>
    ```
    Replace `<post_id>` with the actual post ID.
5.  The generated videos will be stored in the `video_outputs/` directory.

## Configuration

The `config.json` file contains the following configuration settings:

-   `video_width`: Width of the output video.
-   `video_height`: Height of the output video.
-   `character_height_ratio`: Ratio of the character video height to the total video height.
-   `subtitle_font_size`: Font size of the subtitles.
-   `subtitle_width`: Width of the subtitle text box.
-   `padding_top`: Top padding for the character video.
-   `padding_bottom`: Bottom padding for the subtitles.

## Improvements

The following improvements have been made to the codebase:

-   Added more specific exception handling.
-   Improved resource management.
-   Refactored the `process_character` function.
-   Added comments to the code.
-   Moved hardcoded constants to a `config.json` file.

## Notes

-   The `gtts_gen.py` script uses the gTTS library for text-to-speech, which may have limitations.
-   The `moviepy` library is used for video editing, which may require additional dependencies.
-   The `character.json` and `comment.json` files must be in the correct format for the script to work properly.
# video
