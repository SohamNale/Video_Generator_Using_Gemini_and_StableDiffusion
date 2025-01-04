# Video_Generator_Using_Gemini_and_StableDiffusion (Content Machine)

This repository contains two Jupyter notebooks for generating video clips using the Google Gemini model and the Stable Diffusion image generation model. The notebooks can generate videos on any topic, with example prompts provided in the code.

## Notebooks

### Content_Machine_Horizontal.ipynb

This notebook generates horizontal videos with no duration limit. It uses the Google Gemini model for text generation and the Stable Diffusion model for image generation.

#### Features

- Generates horizontal videos on any topic.
- No duration limit for the videos.
- Uses Google Gemini model for text generation.
- Uses Stable Diffusion model for image generation.

#### Example Usage

1. Install the required packages:
    ```sh
    !pip install pydub
    !pip install gtts
    !pip install diffusers --upgrade
    !pip install invisible_watermark transformers accelerate safetensors
    !pip install edge-tts
    !pip install mutagen
    ```

2. Configure the Google Gemini model:
    ```python
    genai.configure(api_key="Use your gemini api key here")
    model = genai.GenerativeModel("gemini-1.5-flash")
    ```

3. Generate video:
    ```python
    video_path = output(text)
    ```

4. Play the video in Colab:
    ```python
    video_path = "final_output.mp4"  # Replace with the actual video path
    play_video_in_colab(video_path)
    ```

### Content_Machine_Vertical.ipynb

This notebook generates vertical videos with a duration limit of under 1 minute. It uses the Google Gemini model for text generation and the Stable Diffusion model for image generation.

#### Features

- Generates vertical videos on any topic.
- Duration limit of under 1 minute for the videos.
- Uses Google Gemini model for text generation.
- Uses Stable Diffusion model for image generation.

#### Example Usage

1. Install the required packages:
    ```sh
    !pip install pydub
    !pip install gtts
    !pip install diffusers --upgrade
    !pip install invisible_watermark transformers accelerate safetensors
    !pip install edge-tts
    !pip install mutagen
    ```

2. Configure the Google Gemini model:
    ```python
    genai.configure(api_key="Use your gemini api key here")
    model = genai.GenerativeModel("gemini-1.5-flash")
    ```

3. Generate video:
    ```python
    video_path = output(text)
    ```

4. Play the video in Colab:
    ```python
    video_path = "final_output.mp4"  # Replace with the actual video path
    play_video_in_colab(video_path)
    ```

## Example Prompts

- Story telling: "You are a professional story teller skilled in adventure, scifi, comedy, fiction, magic, romance, thriller and scary stories."
- Productivity coach: "You are a retired CEO of a multinational tech company who gives advice/tips on any of the given topics ['financial independence', 'productivity', 'time management', 'self improvement', 'mental peace']."
- Facts Teller: "You are a geek and nerd in knowing all the facts related to topics like ['tech fact', 'educational fact', 'funny fact', 'historical fact', 'movie fact', 'scary fact']."
