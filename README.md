# VideoCenter

A tiny GitHub Pages site for clean video playback in Genially. It uses only static files, so there is no Supabase, database, backend, or login layer.

- direct HTTPS video links like `https://legoretro.github.io/VideoCenter/videos/lesson-01.mp4`
- clean player links like `https://legoretro.github.io/VideoCenter/player.html?v=videos/lesson-01.mp4`
- iframe code for Genially with no YouTube branding or ads

## Setup

1. Open `https://github.com/legoretro/VideoCenter`.
2. Upload everything in this folder to the repository root, or push it with Git.
3. Put videos in the `videos/` folder.
4. Edit `videos.json` so the site lists your videos.
5. In GitHub, open `Settings` > `Pages`.
6. Set the source to `Deploy from a branch`, choose `main`, choose `/root`, then save.
7. Open the GitHub Pages URL after it finishes publishing.

Your site URL should be:

```text
https://legoretro.github.io/VideoCenter/
```

## Genially

Use the direct video file when Genially asks for a media URL:

```text
https://legoretro.github.io/VideoCenter/videos/lesson-01.mp4
```

Use the player URL when Genially asks for a web page or embed:

```text
https://legoretro.github.io/VideoCenter/player.html?v=videos/lesson-01.mp4
```

Use iframe code when Genially accepts custom embed code:

```html
<iframe src="https://legoretro.github.io/VideoCenter/player.html?v=videos/lesson-01.mp4" style="width:100%;aspect-ratio:16/9;border:0;" allow="autoplay; fullscreen; picture-in-picture" allowfullscreen></iframe>
```

## Video Format

Use `.mp4` encoded as H.264 video with AAC audio for the best browser support.

## Important Limits

GitHub Pages is good for small public video hosting, but it is not a full video platform.

- Browser uploads to GitHub are limited to 25 MiB per file.
- Normal Git repositories block files over 100 MiB.
- Published GitHub Pages sites have a 1 GB size limit and a soft bandwidth limit.

For large files or lots of viewers, put the video files on storage made for media delivery, then paste those HTTPS file URLs into `player.html`.
