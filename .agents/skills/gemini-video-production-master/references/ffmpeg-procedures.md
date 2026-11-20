# Practical FFmpeg recipes (run only in a trusted terminal with FFmpeg installed)

Probe media:
`ffprobe -v error -show_format -show_streams -of json "input.mp4"`

Create a 10-second 720p preview from second 5 (accurate re-encode):
`ffmpeg -hide_banner -y -ss 5 -i "input.mp4" -t 10 -vf "scale=-2:720,fps=30" -c:v libx264 -preset veryfast -crf 25 -c:a aac -b:a 128k "preview.mp4"`

Find probable silence regions (do not automatically delete):
`ffmpeg -hide_banner -i "input.mp4" -af "silencedetect=noise=-35dB:d=0.5" -f null NUL`

Loudness measurement (2-pass target optional):
`ffmpeg -hide_banner -i "input.mp4" -af loudnorm=I=-16:TP=-1.5:LRA=11:print_format=json -f null NUL`

Create image every 5 seconds for manual inspection:
`ffmpeg -hide_banner -i "input.mp4" -vf "fps=1/5,scale=640:-2" -q:v 4 "frames/frame_%04d.jpg"`

Black frame detection:
`ffmpeg -hide_banner -i "input.mp4" -vf "blackdetect=d=0.2:pix_th=0.10" -an -f null NUL`

Always consider output frame rate, audio sync, subtitle shaping and Windows paths. Avoid shell execution via unsanitized user-controlled filenames. Do not run Windows NUL commands on Linux (use /dev/null).
