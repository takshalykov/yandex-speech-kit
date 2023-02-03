# yandex-speech-kit
Python script for working with Yandex SpeechKit API v1

## Prepare

Install SoX https://sox.sourceforge.net/ and add environment PATH

Register on Yandex Cloud https://cloud.yandex.ru/ and create catalog

Install Yandex CLI https://cloud.yandex.ru/docs/cli/quickstart#install

Get IAM token https://cloud.yandex.ru/docs/iam/operations/iam-token/create

## Run

<code>py main.py --token <IAM_TOKEN> --folder_id <FOLDER_ID> --text "Your text for speech synthesis." --output speech.raw</code>

Convert RAW to WAV

<code>sox -r 48000 -b 16 -e signed-integer -c 1 speech.raw speech.wav</code>

## API Docs

https://cloud.yandex.ru/docs/speechkit/
