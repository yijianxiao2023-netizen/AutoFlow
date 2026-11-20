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
4. About every 10 seconds, new notes show up in that speech's column. Switch speeches as the round goes on.

You can also paste speech text into the side box and click **Flow this text**.

## Flowing by hand
The flow works like a spreadsheet, with or without the AI:
- Click a cell (or move with the arrow keys) and start typing.
- **Enter** saves and moves down. **Tab** moves right. **Esc** cancels.
- **Shift+Enter** adds a new line inside a cell.
- Start a cell with `#` to make it a heading (for example `# Contention 1`).
- **Ctrl/Cmd+Enter** inserts a row and **Ctrl/Cmd+Backspace** deletes one. **Backspace** clears a cell.
- **Ctrl+1–9** picks the current speech, and **Ctrl+Shift+S** adds a sheet (one per off-case, for example).
- Scroll to the bottom to load 1,000 more rows.

## Formats
Policy (CX), Lincoln-Douglas, Public Forum, Parliamentary.

## Notes
- Very fast speaking (spreading) lowers transcription accuracy.
- Check your league's rules on electronics and recording before using this in competition.

## License and credits
AutoFlow is licensed under the **Apache License 2.0**. See [LICENSE](LICENSE) for the full terms.

If you use, copy, modify or distribute AutoFlow, or any project based on it, you must:
1. **Follow the Apache 2.0 license.** Include a copy of the [LICENSE](LICENSE) file and mark any files you changed.
2. **Give credit.** Credit **SlaxY1r ([yijianxiao2023-netizen](https://github.com/yijianxiao2023-netizen))** as the original creator of AutoFlow, with a link back to this repository: https://github.com/yijianxiao2023-netizen/AutoFlow
3. **Keep this README and the [NOTICE](NOTICE) file.** Don't delete them or remove the credits from them.
