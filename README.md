# OpenCV Eigenfaces

Example use of facial recognition using OpenCV's eigenface implementation.

## Usage

	./test_eigenfaces.py

N.B requires a csv file at 
	
	./faces.csv
	
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

## TODO
	[] Improve command line usage to allow file location of csv file, test/training ratio etc.
	
## Credit

This is just a python implementation of some of the behaviour shown in the [OpenCV docs](http://docs.opencv.org/modules/contrib/doc/facerec/facerec_tutorial.html#eigenfaces-in-opencv). 



