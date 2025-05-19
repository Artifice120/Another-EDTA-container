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

Conda has to be initiated each time the image is activated.

The most straight forward way around it is to run the bash script init.bash with the image

The edta command can be added to the end of the bash script itself

```
singularity exec -B /proj/parkerlab/users/jotorr/PaintSHOP_pipeline edta-conda.sif /bin/sh init.bash
```

