# CDlib datasets
<img src="https://cdlib.readthedocs.io/en/latest/_static/cdlib_new.png" alt="CDlib logo" width="100" />


Remote repository of public domain network datasets (along with their ground truth clustering) for the [CDlib](https://github.com/GiulioRossetti/cdlib) libray.

For instructions on how to load the data within CDlib refer to the official [documentation](https://cdlib.readthedocs.io/en/latest/reference/datasets.html)

## Available datasets

Here a list of the available network datasets, both from real and synthetically generated

### Real world 

Network Name | Network Type | Upstream 
------------ | ------------- | -------------
Karate Club | Social | [UCINET](http://vlado.fmf.uni-lj.si/pub/networks/data/Ucinet/UciData.htm)
Youtube | Social | [SNAP](https://snap.stanford.edu/data/com-Youtube.html)
DBLP | Scientific Collaboration | [SNAP](https://snap.stanford.edu/data/com-DBLP.html)
Amazon | Co-Purchases |  [SNAP](https://snap.stanford.edu/data/com-Amazon.html)

### Synthetic 

**LFR Benchmark datasets:** 

Set of networks with planted community partitions generated using the networkx implementation of the Lancichinetti-Fortunato-Radicchi benchmark.
> “Benchmark graphs for testing community detection algorithms”, Andrea Lancichinetti, Santo Fortunato, and Filippo Radicchi, Phys. Rev. E 78, 046110 2008

Dataset names follows the pattern
> LFR_N{number of nodes}_ad{average degree}_mc{min community size}_mu{mixing coefficient}

where: 

- number of nodes: [1000, 5000, 10000, 50000, 100000] 
- average degree: [5]
- min community size: [50]
- mixing coefficient: [0.1, 0.2, 0.3, 0.4, 0.5, 0.6, 0.7, 0.8, 0.9]

The power law exponent for the degree distribution is fixed at 3, while for the community size distribution to 1.5
