# Lyric - Scraper

Lyric-Scraper is a tool to get lyrics for your favourite songs.

## Features

* Can scrape the lyrics from the web by entering Artist and song details.
* Can get the lyrics from meta data of song file.
* Can save the lyrics in file meta data or in text file.
### How To Install
you can directly install from pip.
```
pip3 install lyric-scraper
```
OR

1.) clone this repository
 ```
git clone https://github.com/prakhar1965/lyric-scraper.git
```
2.) Enter into repo's directory
```
cd lyric-scrapper
```
3.)Install the require dependencies by running 
```
pip install -r requirements.txt
```
3.)Install lyric-scrapper by running 
```
python setup.py install
```
### How To Use
* Enter `lyrics` to command prompt, It will ask for artist and song details.
* Enter `lyrics [FILENAMES]`, to get lyric from song MP3 file.
* Check out different options, by enter `lyrics --help`

### Use from python script
```
import sys

sys.path.append("/opt/anaconda3/envs/hack/lib/python3.11/site-packages/")
from lyric_scraper.main import find_lyrics

def main(song_title, song_artist):
    return find_lyrics(song_title, song_artist)

if __name__ == '__main__':
    song_title = "stand by me"
    song_artist = "ben e king"
    lyric = main(song_title, song_artist)
    print("............", lyric)
```

## License

This project is licensed under the MIT License - see the [LICENSE.txt](LICENSE.txt) file for details


