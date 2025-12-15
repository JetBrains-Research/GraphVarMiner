# Status: Archived 

No longer maintained

# GraphVarMiner

## Description

The tool for processing PSI trees from IntelliJ IDEA and creating dataset of contexts for each variable in projects. 
Each context represented in form of graph. How it is built you can see in [Allamanis et al., 2017](https://arxiv.org/abs/1711.00740).

## Usage

To start extracting data run gradle tusk:

```
runIde -Pdataset="datasetDir" -PoutputPrefix="outputPrefix"
```

`datasetDir` is a directory which contains some java projects.
If `outputPrefix="$saveDir\$name"` than you will get a bunch of files like `"$saveDir\$name_$projectName.$numOfArchive.json.gz"`.
