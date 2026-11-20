# Dependency classes and installation boundaries

**Core executable software:** FFmpeg/FFprobe, Python, Node.js, Git, optionally Kdenlive/Blender/Subtitle Edit/Resolve/Premiere; these are not included in Skill ZIPs.
**Python packages:** MoviePy 2, PyAV, OpenCV, PySceneDetect, numpy/scipy, librosa, pydub, pyloudnorm, noisereduce, pysubs2, faster-whisper, WhisperX, pyannote, Ultralytics, supervision, MediaPipe, PyTorch, CLIP/OpenCLIP. Environments may conflict; install selectively in separate venvs.
**Model/research runtime, checkpoints and build dependencies:** SAM 2, Grounding DINO, CoTracker, Depth Anything V2, Video Depth Anything, RIFE, Real-ESRGAN, BasicSR, CodeFormer, GFPGAN, GPT-SoVITS, ComfyUI, Demucs, Video2X. Git clones are not an installation of these models.
**JS/motion:** Remotion/React/TypeScript, Three.js, React Three Fiber/Drei, GSAP, Lottie, anime.js, Motion Canvas, HyperFrames, Manim/Blender (different runtime).
**Editing interchange:** OpenTimelineIO, MLT Framework, GStreamer, MakeMyClip, auto-editor.
**MCP integrations:** locally configured and verified MCP for Adobe Premiere Pro / DaVinci Resolve / FFmpeg. A Skills upload cannot connect these by itself.

Use the full `tool-catalog-80.md` list for URLs and the optional Windows toolchain scripts separately. Check the source's README, license, current branch and platform requirements before enabling a specific integration.
