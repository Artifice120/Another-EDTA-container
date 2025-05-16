# Another-EDTA-container
Container with conda version of EDTA as it seems to be more stable

*Includes singularity/apptainer recipe file for conda install EDTA*

### Install

To download and build with apptainer 

```
git clone https://github.com/Artifice120/Another-EDTA-container/
cd Another-EDTA-container/
apptainer build edta-conda.sif ContainerFile
```

### Run

```
apptainer -B path/to/Another-EDTA-container/ EDTA.pl --genome genome.fa --curatedlib ../database/your.file --overwrite 1 --sensitive 1 --anno 1 --threads 10
```
