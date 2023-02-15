# Fashion Grader

This project leverages machine learning using a dockerized tensorflow environment and data downloader. The datasets are fashion images which can be classified as fashionable or unfashionable.

# Requirements

* [docker](https://www.docker.com/)
* a bash shell

# Project Outline
I trained this model in a dockerized tensorflow environment using Jupyter notebook. 

## Dataset:
I filtered the captioned dataset at https://laion.ai/ to find stylish and unstylish images using the keywords 'new york street style, street style, OOTD, millenial fashion'. These images were downloaded in a JSON format. You can read the JSON into a Dataframe to make the URLs more accessible, then convert them to lists for each data set, stylish/unstylish.

## Downloader: 
I built a custom data downloader that extracted the url from the JSON file, tested the URL for the response status code, and skipped any URLs that where not successful. Images were downloaded from the successful status codes into my data folders: stylish, unstylish, test-images. 

# Final Model

