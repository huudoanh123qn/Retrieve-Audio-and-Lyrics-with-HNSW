## Group member:
* **Nguyen Huu Doanh** - *18520606@gm.uit.edu.vn*
* **Nguyen Minh Châu** - *18520519@gm.uit.edu.vn*
* **Tô Viết Anh** - *18520471@gm.uit.edu.vn*
## Introduction
This project is on the field of Computer Vision, an sub-domain of Computer Science. On this project, we build our audio and lyrics retrieval system based on the paper [Efficient and robust approximate nearest neighbor search using hierarchical navigable small world graphs]

This our system has 3 parts:

* Music Query
* Lyric Query
* Keyword Query
Futhermore, we use [Flask](https://flask.palletsprojects.com/en/1.1.x/) - an web framework using for python to build our GUI
## Report

Our report is below:

[Report](Report.pdf)

## Demo
### Main screen

![alt text](https://github.com/huudoanh123qn/Retrieve-Audio-and-Lyrics-with-HNSW/tree/master/static/images/main.jpg)
![alt text](https://github.com/huudoanh123qn/Retrieve-Audio-and-Lyrics-with-HNSW/tree/master/static/images/main1.jpg)

### Example Example retrieval

![alt text](https://github.com/huudoanh123qn/Retrieve-Audio-and-Lyrics-with-HNSW/tree/master/static/images/demo1.jpg)
![alt text](https://github.com/huudoanh123qn/Retrieve-Audio-and-Lyrics-with-HNSW/tree/master/static/images/demo2.jpg)

## Pre Proccessing

Prepare musics + images(albums) + lyrics path.

**NOTES:**
* Images: Put in ./static/ images/ path.
* All of musics, images, lyrics of 1 song must have same name.

## 1. Activate environment

    ./env/Scripts/activate

## 2. Create necessary file

* Create musics model:

      python build_model.py --data-dir"./data"

      --data-dir: directory of music with .mp3/wav extension.

* Create lyrics model:

      python ./utils/lyrics_inverted_file.py

* Create song keyword model:

      python ./utils/create_songs_db.py

    
## 3. Run music query's website

    python app.py
    
