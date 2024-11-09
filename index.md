# HI!
## This are some changes!!
- some text
- more text
  - sub
  - more sub
- final
### sub-changes
- [x] **step 1**
- [x] **step 2**
- [x] **step 3**
- [x] step 4 (current)
- [ ] _step 5_

first|second
-|-
2|3
4|9
6|1

#### XD
![cool wallpaper](https://th.wallhaven.cc/lg/3l/3lp2md.jpg)
#### Code
##### normal code with `pass`
```
$ pass
Password Store
├── deezer_arl
└── github
```
##### `python` code
``` python
import re

def process_file(input_file, output_file):
    with open(input_file, 'r') as file:
        input_string = file.read()

    # Adjust the pattern to handle the single-line input correctly
    pattern = re.compile(r'(\d+\.\s.*?\.flac)(small\.fileditchstuff\.me\/s..\/[a-zA-Z0-9]+\.flac)')
    matches = pattern.findall(input_string)
    result = []

    for match in matches:
        song_info, url = match
        # Extract the title by removing everything inside the square brackets and the .flac extension
        song_title = re.sub(r'\s*\[.*?\]', '', song_info).strip()
        song_title = re.sub(r'^\d+\.\s*', '', song_title)  # Remove leading number and dot
        song_title = re.sub(r'\.flac$', '', song_title)  # Remove trailing .flac
        formatted_url = "https://" + url
        result.append(f"{formatted_url} {song_title}")

    with open(output_file, 'w') as file:
        for line in result:
            file.write(line + '\n')

# Input and output file names
input_file = 'songs.txt'
output_file = 'formatted_songs.txt'

# Process the file
process_file(input_file, output_file)

print(f"Formatted data has been written to {output_file}")
```
##### Bye
