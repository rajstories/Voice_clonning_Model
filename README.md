# 🎙️ AI Voice Cloning Tool

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/YOUR_USERNAME/YOUR_REPO_NAME/blob/main/Voice_Cloning_Notebook.ipynb)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python 3.9+](https://img.shields.io/badge/python-3.9+-blue.svg)](https://www.python.org/downloads/)

A powerful, free, and easy-to-use voice cloning tool for content creators. Clone your voice with just a 15-30 second audio sample and generate unlimited voiceovers for your content.

## ✨ Features

- 🎯 **High-Quality Voice Cloning** - Clone your voice with just 15-30 seconds of audio
- 🌍 **Multi-Language Support** - Works with Hindi, English, and 15+ other languages
- 🆓 **100% Free** - Uses Google Colab's free GPU resources
- 🚀 **Fast Generation** - Generate voiceovers in 20-30 seconds
- 💻 **No Coding Required** - Simple web interface, just upload and type
- 🎨 **Content Creator Friendly** - Perfect for YouTube, podcasts, and social media

## 📋 Table of Contents

- [Quick Start](#-quick-start)
- [Requirements](#-requirements)
- [Installation](#-installation)
- [Usage](#-usage)
- [Supported Languages](#-supported-languages)
- [Tips for Best Results](#-tips-for-best-results)
- [Troubleshooting](#-troubleshooting)
- [Use Cases](#-use-cases)
- [Contributing](#-contributing)
- [License](#-license)
- [Acknowledgments](#-acknowledgments)

## 🚀 Quick Start

### Option 1: Google Colab (Recommended)

1. Click the "Open in Colab" badge above
2. Run all cells: `Runtime` → `Run all`
3. Wait 3-4 minutes for setup
4. Click the generated link
5. Upload your voice, type your script, and generate!

### Option 2: Local Setup

```bash
# Clone the repository
git clone https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git
cd YOUR_REPO_NAME

# Install dependencies
pip install TTS gradio torch

# Run the notebook
jupyter notebook Voice_Cloning_Notebook.ipynb
```

## 📦 Requirements

- Python 3.9 - 3.11 (Note: Python 3.12+ not supported by TTS library)
- GPU recommended (Google Colab provides free GPU)
- 15-30 seconds of clear voice recording
- Basic understanding of running Jupyter notebooks

### Python Packages

```
TTS==0.22.0
gradio>=4.0.0
torch>=2.0.0
```

## 💻 Installation

### Google Colab (No Installation Required)

Simply open the notebook in Colab - all dependencies are installed automatically!

### Local Installation

```bash
# Create virtual environment (recommended)
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install requirements
pip install -r requirements.txt

# Launch Jupyter
jupyter notebook
```

## 📖 Usage

### Step 1: Prepare Your Voice Sample

Record a clear 15-30 second audio clip:

```
✅ DO:
- Record in a quiet room
- Speak naturally (like you normally do)
- Use a decent microphone (phone mic is fine)
- Save as WAV or MP3

❌ DON'T:
- Record with background noise/music
- Whisper or shout
- Use heavily compressed audio
- Include multiple speakers
```

### Step 2: Run the Notebook

```python
# After running all cells, you'll see:
# 1. Audio upload box
# 2. Reference text field
# 3. Generation text field
# 4. Language selector
```

### Step 3: Generate Your Cloned Voice

1. **Upload your audio file**
2. **Enter reference text** (what you said in the recording)
   ```
   Example: "Hello everyone! My name is Raj and this is my channel."
   ```
3. **Enter generation text** (new content you want)
   ```
   Example: "Today we'll discuss artificial intelligence and voice cloning."
   ```
4. **Select language** (hi for Hindi, en for English)
5. **Click Submit** and wait 20-30 seconds
6. **Download** your cloned voice!

## 🌍 Supported Languages

| Language | Code | Quality |
|----------|------|---------|
| English | en | ⭐⭐⭐⭐⭐ |
| Hindi | hi | ⭐⭐⭐⭐⭐ |
| Spanish | es | ⭐⭐⭐⭐⭐ |
| French | fr | ⭐⭐⭐⭐⭐ |
| German | de | ⭐⭐⭐⭐⭐ |
| Italian | it | ⭐⭐⭐⭐ |
| Portuguese | pt | ⭐⭐⭐⭐ |
| Polish | pl | ⭐⭐⭐⭐ |
| Turkish | tr | ⭐⭐⭐⭐ |
| Russian | ru | ⭐⭐⭐⭐ |
| Dutch | nl | ⭐⭐⭐⭐ |
| Czech | cs | ⭐⭐⭐⭐ |
| Arabic | ar | ⭐⭐⭐⭐ |
| Chinese | zh-cn | ⭐⭐⭐⭐ |
| Japanese | ja | ⭐⭐⭐⭐ |
| Hungarian | hu | ⭐⭐⭐ |
| Korean | ko | ⭐⭐⭐ |

## 💡 Tips for Best Results

### Recording Quality

```
📱 Good Recording Setup:
- Quiet room (no AC, fan, traffic noise)
- 1-2 feet from microphone
- Phone voice recorder is sufficient
- WAV format preferred (but MP3 works)
- 16kHz+ sample rate
```

### Reference Text

```
✅ IMPORTANT: Reference text must EXACTLY match your audio

❌ Wrong:
Audio: "Hello everyone, welcome to my channel!"
Text: "Hi everyone, welcome to my channel!"

✅ Correct:
Audio: "Hello everyone, welcome to my channel!"
Text: "Hello everyone, welcome to my channel!"
```

### Generation Text

```
✅ DO:
- Write naturally (as you'd normally speak)
- Use proper punctuation for pauses
- Keep sentences reasonable length
- Use Roman script for Hindi (better results)

❌ DON'T:
- Write extremely long paragraphs
- Use complex technical jargon unnecessarily
- Mix multiple languages heavily
```

### Language-Specific Tips

**For Hindi/Hinglish:**
```
✅ Use Roman script: "Namaste doston"
❌ Avoid Devanagari in text: "नमस्ते दोस्तों"

Reason: The model processes Roman script more accurately
```

**For English:**
```
✅ Natural: "Hey guys, what's up?"
❌ Robotic: "Hello. How. Are. You."
```

## 🔧 Troubleshooting

### Common Issues and Solutions

#### Issue: "Voice doesn't sound like me"

**Solutions:**
1. ✅ Verify reference text EXACTLY matches your audio
2. ✅ Use longer reference audio (25-30 seconds better than 10)
3. ✅ Re-record with clearer pronunciation
4. ✅ Ensure your reference audio has minimal background noise

#### Issue: "Hindi pronunciation is incorrect"

**Solutions:**
1. ✅ Use Roman script: "Namaste doston" ✓
2. ❌ Don't use Devanagari: "नमस्ते दोस्तों" ✗
3. ✅ Make sure language is set to 'hi'
4. ✅ Avoid very complex Sanskrit words in first attempts

#### Issue: "Audio quality is poor/robotic"

**Solutions:**
1. ✅ Record in quieter environment
2. ✅ Use better microphone or phone closer to mouth
3. ✅ Use WAV format instead of compressed MP3
4. ✅ Ensure reference audio is at least 15 seconds long

#### Issue: "Installation fails on Python 3.12+"

**Solution:**
```bash
# TTS library requires Python < 3.12
# Use Python 3.11 or earlier
conda create -n voice-clone python=3.11
conda activate voice-clone
pip install TTS gradio
```

Or use **Google Colab** which has compatible Python version.

#### Issue: "CUDA/GPU not detected"

**Solutions:**
1. For Colab: `Runtime` → `Change runtime type` → Select `T4 GPU`
2. For local: Install CUDA toolkit matching your PyTorch version
3. CPU mode works but is slower (60-90 seconds per generation)

#### Issue: "ModuleNotFoundError: No module named 'TTS'"

**Solution:**
```bash
# Make sure you ran the installation cell first
pip install TTS --upgrade
```

## 🎯 Use Cases

### Content Creators
- Generate voiceovers for YouTube videos without recording
- Create multiple language versions of content
- Save time on re-recording corrections
- Maintain consistent voice quality across videos

### Podcasters
- Generate audio snippets for social media
- Create preview clips
- Automate voice segments

### Educators
- Create educational content in multiple languages
- Generate voice for e-learning materials
- Personalize student feedback

### Businesses
- Create voice messages for customers
- Generate IVR messages
- Localize content for different markets

## 📊 Performance Benchmarks

| Hardware | Generation Time (10 sec audio) |
|----------|--------------------------------|
| Google Colab T4 GPU | ~20 seconds |
| NVIDIA RTX 3080 | ~15 seconds |
| CPU (i7-10700K) | ~90 seconds |

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. 🐛 **Report bugs** - Open an issue with details
2. 💡 **Suggest features** - Share your ideas
3. 📝 **Improve docs** - Fix typos, add examples
4. 🔧 **Submit PRs** - Fix bugs or add features

### Development Setup

```bash
git clone https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git
cd YOUR_REPO_NAME
pip install -e .
pytest tests/
```

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- [Coqui TTS](https://github.com/coqui-ai/TTS) - Excellent TTS library
- [XTTS v2](https://huggingface.co/coqui/XTTS-v2) - Voice cloning model
- [Gradio](https://gradio.app/) - User interface framework
- Google Colab - Free GPU resources

## ⚠️ Ethical Considerations

**Please use this tool responsibly:**

✅ **DO:**
- Clone your own voice for your content
- Get explicit permission before cloning someone else's voice
- Clearly disclose when audio is AI-generated
- Use for legitimate content creation

❌ **DON'T:**
- Impersonate others without permission
- Create misleading or harmful content
- Use for fraud, scams, or illegal activities
- Violate anyone's rights or privacy

**Remember: With great power comes great responsibility.**

## 📞 Support

- 🐛 Issues: [GitHub Issues](https://github.com/YOUR_USERNAME/YOUR_REPO_NAME/issues)
- 💬 Discussions: [GitHub Discussions](https://github.com/YOUR_USERNAME/YOUR_REPO_NAME/discussions)
- 📧 Email: your.email@example.com

## 🗺️ Roadmap

- [ ] Add batch processing for multiple scripts
- [ ] Integrate emotion control
- [ ] Support for more languages
- [ ] Fine-tuning capabilities
- [ ] API endpoint for integration
- [ ] Desktop application
- [ ] Mobile app

## 📈 Stats

![GitHub stars](https://img.shields.io/github/stars/YOUR_USERNAME/YOUR_REPO_NAME?style=social)
![GitHub forks](https://img.shields.io/github/forks/YOUR_USERNAME/YOUR_REPO_NAME?style=social)
![GitHub watchers](https://img.shields.io/github/watchers/YOUR_USERNAME/YOUR_REPO_NAME?style=social)

---

<div align="center">

**Made with ❤️ for Content Creators**

⭐ Star this repo if you find it useful!

[Report Bug](https://github.com/YOUR_USERNAME/YOUR_REPO_NAME/issues) · [Request Feature](https://github.com/YOUR_USERNAME/YOUR_REPO_NAME/issues) · [Documentation](https://github.com/YOUR_USERNAME/YOUR_REPO_NAME/wiki)

</div>
