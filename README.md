# VideoCenter

Static GitHub Pages video hosting. No Supabase, no database, no YouTube ads.

Open the helper page:

```text
https://legoretro.github.io/VideoCenter/
```

Upload videos here:

```text
https://github.com/legoretro/VideoCenter/upload/main/videos
```

The helper page automatically lists the uploaded video files and gives you copy buttons for:

- clean player URLs
- raw file URLs
- iframe embed codes for Genially

Clean player link pattern:

```text
https://legoretro.github.io/VideoCenter/player.html?v=VIDEO-SOURCE
```

Use `.mp4` with H.264 video and AAC audio for best browser support.

If Genially shows `null` for a plain video URL, use the helper page's `Embed code` button instead. The player and embed options use the raw GitHub file behind the scenes, so they can work even while GitHub Pages is still updating direct `/videos/...` links.
