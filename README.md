# Segmented anisotropic ssTEM dataset of neural tissue

The ground truth stack 1 contains 20 sections from serial section Transmission Electron Microscopy (ssTEM) of the Drosophila melanogaster third instar larva ventral nerve cord. The cube measures 4.7 x 4.7 x 1 microns approx, with a resolution of 4.6 x 4.6 nm/pixel and section thickness of 45-50 nm.

You are free to use this data set for the purpose of generating or testing non-commercial image segmentation software. If any scientific publications derive from the usage of this data set, you must cite:

*Segmented anisotropic ssTEM dataset of neural tissue.* Stephan Gerhard, Jan Funke, Julien Martel, Albert Cardona, Richard Fetter. figshare. Retrieved 16:09, Nov 20, 2013 (GMT) http://dx.doi.org/10.6084/m9.figshare.856713


```bibtex
@article{Gerhard2013vncgroundtruth,
	Author = {Stephan Gerhard and Jan Funke and Julien Martel and Albert Cardona and Richard Fetter},
	Date-Added = {2017-06-29 04:35:14 +0000},
	Date-Modified = {2017-06-29 05:32:12 +0000},
	Journal = {figshare},
	Title = {Segmented anisotropic ssTEM dataset of neural tissue},
	Url = {http://dx.doi.org/10.6084/m9.figshare.856713},
	Volume = {http://dx.doi.org/10.6084/m9.figshare.856713},
	Year = {2013},
	Bdsk-Url-1 = {http://dx.doi.org/10.6084/m9.figshare.856713}}
```

### Content
  
```
├── stack1
│   ├── raw: The raw 8-bit greyscale images
│   ├── membranes: Series of binary images of segmented membranes
│   ├── mitochondria: Series of binary images of segmented mitochondria
│   ├── synapses: Series of binary images of segmented synapses
│   └── labels: Series of merged labels including membranes, mitochondria, synapses as separate channels
└── stack2
    └── raw: The raw 8-bit greyscale images
```

### Modifications

The following modifications have been applied to the orginal dataset:
- All images are converted to portable network graphics (png) format
- All file names are numbers 00~19
- Labels contain a combination of membranes, mitochondria, synapses. For oriented membranes, junctions, glia/extracellular space etc. see original dataset.

### TODO

Three-dimensional segmentation into neurons/regions.

## Original

Repository: [Segmented anisotropic ssTEM dataset of neural tissue](https://github.com/unidesigner/groundtruth-drosophila-vnc)

Contact: [Stephan Gerhard](mailto:git@unidesign.ch)

### The challenge
Use *stack 1* to train pixel classifiers for the purpose of automatic segmentation of neural structures in ssTEM. For instance, use 80% of the sections to train, and 20% of the sections for validation. Apply the classifier to the raw data of *stack 2* (test data) and send us the results, so we're able to compute pixel-wise and other error measures in the subsequent neuron reconstruction pipeline.

### License
This work is licensed under a
[Creative Commons Attribution-NonCommercial-ShareAlike 3.0 Unported License.](http://creativecommons.org/licenses/by-nc-sa/3.0/deed.en_US)
<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/3.0/deed.en_US"><img alt="Creative Commons License" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/3.0/88x31.png" /></a>

