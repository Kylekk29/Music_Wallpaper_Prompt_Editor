**English** | [简体中文](README.zh-CN.md)

# Music Wallpaper Prompt Editor

A single-file, offline HTML tool that builds a detailed image-generation prompt for turning
your own photo into a phone wallpaper styled like the **Apple Music** or **Spotify**
"Now Playing" screen. The prompt is written in Traditional Chinese (Hong Kong style).

The tool does **not** generate images, call any API, or connect to Apple Music / Spotify.
It only assembles text. You paste that text into an image-capable chat (for example ChatGPT)
together with your original photo.

## Usage

1. Open `index.html` in any modern browser (no install, no server, no dependencies).
2. Choose the **music platform** (Apple Music or Spotify).
3. Fill in the song, artist, aspect ratio, photographic style and the optional switches.
4. The full prompt updates live on the right. You can edit the text directly.
5. Click **複製提示詞** (copy), or **複製並開啟 ChatGPT** (copy and open ChatGPT), then upload
   your photo and paste the prompt.

## Options

| Group | Options |
|---|---|
| Platform | Apple Music, Spotify |
| Aspect ratio | 9:16, 3:4, 1:1, 4:5, 2:3, 9:19.5, 16:9 |
| Photographic style | 10 presets (cinematic sunset, film, night, golden hour, blue hour, ...) |
| Interface text | Traditional Chinese, English, original song data + Traditional Chinese UI |
| UI text colour | White, dark, automatic |
| UI position | Bottom, top, centred-low with gradient |
| Background | Keep, slight blur, vignette + gradient |
| Accent colour | Platform accent (red / green): small, none, more |
| Toggles | keep accessories, extend background, album art rule, status bar, lock-screen clock, no watermark, keep sharp detail |
| Extras | free-text extra requirements, `.txt` download |

## Sample prompts

Full generated output with the default settings (song 轉眼, artist 五月天, 9:16, cinematic sunset):

- [`examples/apple-music-sample-prompt.txt`](examples/apple-music-sample-prompt.txt)
- [`examples/spotify-sample-prompt.txt`](examples/spotify-sample-prompt.txt)

## Notes and limitations

- The interface layouts are written from public descriptions of the iOS Apple Music and
  Spotify Now Playing screens. The image model may not reproduce them exactly.
- Playback times in the prompt are decorative only, not real playback data.
- Apple Music and Spotify are trademarks of their respective owners. This project is
  independent and not affiliated with or endorsed by Apple or Spotify.

## License

[MIT](LICENSE)
