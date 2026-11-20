# AutoFlow

A free AI debate flow that listens through your mic and flows the round for you. Everything runs in your browser: no server, no API key, no account.

**Live site:** https://yijianxiao2023-netizen.github.io/AutoFlow/

## How it works
- **Mic → text:** the browser's built-in speech recognition (best in Chrome).
- **Text → flow:** a small AI model (Qwen 2.5 or Llama 3.2) running on your own computer through [WebLLM](https://github.com/mlc-ai/web-llm) and WebGPU. The model downloads once (about 1–2 GB) and stays saved in your browser.
- **Flow:** a column for each speech, with every answer lined up next to the argument it responds to. Notes can be edited, and the flow is saved in your browser.

## Using it
1. Open the site in a recent version of **Chrome** on a computer with a decent graphics chip (Apple Silicon Macs work well).
2. Click **Load model**. Only the first load is slow.
3. Pick the format and the speech that's about to start, then press **Record**.
4. About every 15 seconds, new notes show up in that speech's column. Switch speeches as the round goes on.

You can also paste speech text into the side box and click **Flow this text**.

## Formats
Policy (CX), Lincoln-Douglas, Public Forum, Parliamentary.

## Notes
- Very fast speaking (spreading) lowers transcription accuracy.
- Check your league's rules on electronics and recording before using this in competition.
