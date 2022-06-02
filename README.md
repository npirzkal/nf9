# nf

A high level module to allow one to quickly display images from Python that relies on the pyds9 module (https://github.com/ericmandel/pyds9)


# Installing: #
```
pip install nf
```

or clone github depo and
```
python setup.py install
```

# Sample Usage: #
```
import nf

# Display a file
nf.disp("file.fits",1)

# arr = np.ones((100,100))
nf.disp(arr,1)

# Display catalog in DS9
xs = [10,100,20]
ys = [20,20,100]
nf.tvm(x=xs,y=ys,frame=1,circle=20, color='Red')

# Read value from DS9
i,j,v = nf.imexam(frame=1) 
```