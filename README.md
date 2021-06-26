# MTV-YTDLP

### **Description:**
Auto Merge MTV.com Episode output from multiple MP4 files in to a SINGLE MP4. 

MTV.com episodes are split in to multiple MP4 files, so the resulting output for a single episode can be between 3-11+ MP4 files.
This script is a band-aid for that.


### **TL;DR:**

MTV-YTDLP is a Simple script that uses YT-DLP do download an episode from MTV.com, and then merge the resulting multiple output MP4 files using ffmpeg.



### **Installing & Using MTV-YTDLP:**

**Step One: Clone The Repo**

`git clone https://github.com/ohmybahgosh/MTV-YTDLP.git && cd MTV-YTDLP`


**Step Two: Copy to /usr/local/bin and make script executable**

`sudo cp MTV-YTDLP /usr/local/bin/MTV-YTDLP && sudo chmod +x /usr/local/bin/MTV-YTDLP`


**Step Three: Run MTV-YTDLP:**

MTV-YTDLP uses input as variables via the CLI

The first input variable ($1) will be the MTV.COM episode url.  

The second input variable ($2) will be the final merged MP4 output filename. Be sure to **wrap the desired output name in double quotes (““)** and you **MUST** include the **.mp4** extension.


**Example Command:**
`MTV-YTDLP https://www.mtv.com/episodes/viogcs/jersey-shore-family-vacation-welcome-to-the-poconos-season-4-ep-18 "Jersey Shore Family Vacation - S04E18.mp4"`



## **NOTE:**
Not to be confused with ".part.mp4" output files. MTV.com episodes will output MULTIPLE FINISHED MP4 files, each with unique names.  These output files are not temporary files, but the actually final output. So the purpose of this shitty script is to merge them in to a single final episode MP4.

