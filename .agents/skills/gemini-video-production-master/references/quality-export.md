# Video QA and export standards

- Verify via `ffprobe`: real width/height, stream timestamps, duration, fps, audio codec, video codec and color tags.
- Validate no unintended black frames, silent channels, clipping, color flicker, subtitle overlaps, watermark/brand logo distortion, or UI crops.
- For Instagram Reels/TikTok vertical use 9:16 layout; typical authored output 1080×1920 (but re-check current platform rules).
- For landscape reference use 16:9 1920×1080 unless the brief specifies UHD or alternate dimension.
- Caption safe zones: account for actual app UI, action bar, description and bottom navigation; review an on-device mockup.
- For professional deliveries keep separate review MP4 and original-quality archival master as justified.
- Never guarantee 4K quality from a low-resolution source without caveating reconstructed pixels and artifacts.
- Save final checksums, delivery manifest, licensed-music credits, and approved copy.
