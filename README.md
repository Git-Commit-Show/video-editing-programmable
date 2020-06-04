# Programmable video editing
## Scripts, tools and resources to automate video editing

### Scripts

1. [autocut: Cut video at specified timestamps](/autocut.sh)  `autocut infile timestamp1 timestamp2 ...`
2. [combine: Combine multiple videos into one - quite slow but it doesn't have audio/video sync issue](/combine.sh) `combine fileList.txt`
3. [combinevideos: Combine multiple videos into one (fast but works only when all files format, timescale and fps are same)](/combinevideos.sh) `combinevideos fileList.txt`
4. [recordscreen: Record screen using ffmpeg](/recordscreen.sh) `recordscreen`
5. [removeduplicateframes: Reduce frame rate and size by removing duplicate frames](/removeduplicateframes.sh) `removeduplicateframes mybigvideofile.mp4`

**How to use scripts on linux**

1. Download the scripts and go to your terminal
2. Open `~/.bashrc`  with command `sudo gedit ~/.bashrc`
3. Append the content of the script (e.g. content of autocut script) to `~/.bashrc` inside a function as follows
```
autocut() {
  #Content of autocut script goes here
}
```
3. Run `source ~/.bashrc`
4. Now you will be able to run the command `autocut infilepath timestamp1 timestamp2`
