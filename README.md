# Subtitle Translator

<img width="780" src="https://github.com/tvone/subtitle-translator-electron/blob/master/assets/subtitle_electron.PNG">
<p align="center">
  Translate subtitle using ChatGPT
</p>

## How to custom model, temperature and top_p
- Find file .env in the root of the app and change it
- Example : CUSTOM_MY_MODEL=gpt-4-1106-preview
- gpt-4-1106-preview is model name

<img width="251" src="https://github.com/tvone/subtitle-translator-electron/blob/master/assets/custom_env.PNG">

## Why custom temperature and top_p

Nucleus sampling is a technique used in large language models to control the randomness and diversity of generated text. It works by sampling from only the most likely tokens in the model’s predicted distribution.<br />
The key parameters are:

- Temperature: Controls randomness, higher values increase diversity.

- Top-p (nucleus): The cumulative probability cutoff for token selection. Lower values mean sampling from a smaller, more top-weighted nucleus.

In general:

- Higher temperature will make outputs more random and diverse.

- Lower top-p values reduce diversity and focus on more probable tokens.

OpenAI recommends only altering either temperature or top-p from the default.<br />

Temperature and Top_p have a default of 1

## Supported subtitle extensions

- `.ass`
- `.srt`
- `.ssa`
- `.vtt` WebVTT

## Features

- Translate subtitle using ChatGPT
- Support multiple languages
- Translation according to the preceding and following sentences

Thank you gnehs