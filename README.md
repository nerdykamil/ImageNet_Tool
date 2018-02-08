# ImageNet_Tool


This provides a way of downloading images provided the urls from imagenet website
from image net website you can get the urls and boundingboxes but to download the 
images with same name as boundingboxes do following:

clone the repository and extract it to a folder

goto:
http://image-net.org/synset?

browse to the category you want to download the images for,
get 'wnid' by clicking on Wordnet IDs on top right
 
now insert 'wnid' in link below, copy all text and save it in a file (eg. images_url.txt)
http://www.image-net.org/api/text/imagenet.synset.geturls.getmapping?wnid=[wnid] 

navigate to the repository directory you extracted create a new folder [images]
open terminal in repository directory and run:

$ python download_imagenet_images.py --u '/path/to/images_url.txt' --o './images

