# OpenCV Eigenfaces

Example use of facial recognition using OpenCV's eigenface implementation.

## Usage

	./test_eigenfaces.py

N.B requires a csv file at 
	
	./faces.csv
	
##Dependencies
[OpenCV](http://opencv.org/)
```bash
brew install opencv
```

Create your virtualenv allowing for site packages, so you can access opencv python bindings

```bash
virtualenv --system-site-packages
```

Then install deps from requirements.txt
```bash
pip install -r requirements.txt
```

## Preparation
	
I used the set of example face images available from [AT&T Labs Database of Faces](http://www.cl.cam.ac.uk/research/dtg/attarchive/facedatabase.html).

```bash	
wget http://www.cl.cam.ac.uk/Research/DTG/attarchive/pub/data/att_faces.tar.Z \
&& uncompress att_faces.tar.Z \
&& tar xvf att_faces.tar
```
	
Create the necessary csv file
	
```bash
./create_csv.py orl_faces > faces.csv
```

This will create a csv in the form file;label. See [OpenCV Docs](http://docs.opencv.org/modules/contrib/doc/facerec/facerec_tutorial.html#creating-the-csv-file) for more info.

## Credit

This is just a python implementation of some of the behaviour shown in the [OpenCV docs](http://docs.opencv.org/modules/contrib/doc/facerec/facerec_tutorial.html#eigenfaces-in-opencv). 



