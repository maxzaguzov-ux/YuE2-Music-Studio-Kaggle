# 🎵 YuE2 Music Studio - Kaggle Notebooks

AI-powered text-to-music generation using YuE2 model with ComfyUI backend.

## 🚀 Choose Your Interface

### Option 1: Native Forms (Simple & Lightweight)
Classic Jupyter notebook interface with built-in forms. No external servers needed.

[![Open in Kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://www.kaggle.com/kernels/welcome?src=https://github.com/maxzaguzov-ux/YuE2-Music-Studio-Kaggle/blob/main/yue2-music-studio-no-gradio.ipynb)

### Option 2: Gradio Web UI (Advanced & Interactive)
Full web interface with real-time progress tracking and modern design.

[![Open in Kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://www.kaggle.com/kernels/welcome?src=https://github.com/maxzaguzov-ux/YuE2-Music-Studio-Kaggle/blob/main/yue2-text2music-kaggle.ipynb)

---

## 📝 Features

Both versions include:
- 🎼 **5 Genre Presets**: Indie Pop, Synthwave, Lo-Fi, Cinematic, Alt Rock
- ✍️ **Custom Lyrics**: Support for `[Verse]`, `[Chorus]`, `[Bridge]`, `[Outro]` structure
- ⚙️ **Advanced Controls**: Sampler, scheduler, steps, seed, ABC planning
- 🎧 **Real-time Progress**: Live progress bar during generation
- 📥 **Easy Download**: Built-in audio player and batch ZIP download

### Version Differences

| Feature | Native Forms | Gradio Web UI |
|---------|--------------|---------------|
| **Interface** | Jupyter cells with forms | Full web application |
| **Setup** | Simpler, no extra dependencies | Requires Gradio installation |
| **Progress** | Text-based in cell output | Visual progress bar in UI |
| **Audio Player** | HTML5 player in cell | Integrated audio component |
| **Best for** | Quick generation, minimal setup | Repeated use, better UX |

---

## 🛠️ Requirements

- **GPU**: T4 x2 or P100 (recommended)
- **Internet**: Enabled (for model download ~7.26 GB)
- **Storage**: ~10 GB free space
- **Runtime**: ~30 minutes per session

---

## 📖 How to Use

### For Native Forms Version:
1. Click the first "Open in Kaggle" button above
2. Enable GPU: **Settings → Accelerator → GPU T4 x2**
3. Enable Internet: **Settings → Internet → ON**
4. Run cells 1-3 to set up environment and download model
5. Run cell 4. **Click "Show form" icon** (list/sliders) on the left side of the cell
6. Configure your music parameters and run the cell
7. Use cell 5 to download all generated tracks

### For Gradio Web UI Version:
1. Click the second "Open in Kaggle" button above
2. Enable GPU and Internet (same as above)
3. Run cells 1-3 to set up environment
4. Run cell 4 to launch Gradio interface
5. **Click the public link** (`.gradio.live`) that appears in the output
6. Use the web interface to configure and generate music
7. Download tracks directly from the interface

---

## 🎨 Interface Examples

### Native Forms
- Clean, minimal interface
- All parameters in collapsible form fields
- Output displayed directly in notebook cells

### Gradio Web UI
- Modern, responsive design
- Real-time progress visualization
- Integrated audio player with download button
- Better for repeated use sessions

---

## 📄 License & Credits

This notebook is adapted from [AI With Chucky](https://github.com/AICHUCKY/Ai-with-Chucky-Colab-Notebooks) for the Kaggle platform.

- **Original notebook**: [AI With Chucky](https://github.com/AICHUCKY/Ai-with-Chucky-Colab-Notebooks/blob/main/Yue2_text2music.ipynb)
- **Model**: [YuE2 FP16](https://huggingface.co/Jokality/YuE2-fp16) by Jokality
- **Framework**: [ComfyUI](https://github.com/comfyanonymous/ComfyUI)
- **Web UI**: [Gradio](https://gradio.app/) (for Gradio version)

---

## 🐛 Troubleshooting

### Common Issues:
1. **"GPU Not Detected"** → Enable GPU in Settings → Accelerator
2. **"No output file found"** → Check that cell 3 completed successfully (🟢 message)
3. **Gradio link not working** → Make sure Internet is enabled in Settings
4. **Model download fails** → Check Internet connection, retry cell 3

### Tips:
- **Disable ABC Planning** for faster generation (saves 2-3 minutes)
- **Use `[Outro]` tag** at the end of lyrics for proper song ending
- **Randomize seed** for different variations of the same prompt
- **Save your notebook** after successful generation to preserve outputs

---

## 📊 Performance

- **Model size**: ~7.26 GB (FP16)
- **Generation time**: 3-5 minutes (without ABC), 5-8 minutes (with ABC)
- **VRAM usage**: ~8-10 GB
- **Output format**: MP3, WAV, or FLAC (user selectable)

---

**Happy music making! 🎵**
