# Bumfy

single-file minimal frontend for ComfyUI

## Quick start

- Use online: https://antiven0m.github.io/bumfy/
- Local use: open `index.html` in a browser.
- Mobile mode: planned.

## ComfyUI CORS header (Windows .bat)

This UI talks to ComfyUI. Enable CORS in your ComfyUI launch script:

1. Open your ComfyUI launch `.bat` (for example `run_nvidia_gpu.bat`).
2. Add `--enable-cors-header` to the `python main.py` line.

Example:

```bat
.\python_embeded\python.exe -s ComfyUI\main.py --windows-standalone-build --enable-cors-header
```
This flag allows browser requests to reach ComfyUI without CORS errors.

> [!IMPORTANT]
> Use CORS only with tools you trust, and double-check the source before letting anything talk to your ComfyUI instance.
