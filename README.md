# yt-dl-action

GitHub Actions powered YouTube downloader. Downloads videos via yt-dlp on GitHub's servers, then uploads as artifacts.

## Usage

### Method 1: Manual trigger (single URL)

1. Go to **Actions** tab → **YouTube Downloader** → **Run workflow**
2. Paste the YouTube URL
3. Check "Extract audio only" if you only need MP3
4. Click **Run workflow**
5. Download the artifact from the completed run

### Method 2: Batch via playlist.txt

1. Edit `playlist.txt` and add video URLs (one per line)
2. Commit and push
3. Download the artifact from the triggered run

### Artifact retention

Artifacts are kept for **7 days**. Download them before they expire.

## Why

The Hana sandbox blocks direct YouTube connections. GitHub Actions runners can reach YouTube and run yt-dlp without restrictions.
