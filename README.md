# TFM
scripts and data examples of my master's thesis

inside of counting_particles, there are available two python scripts:
- **num_particles.ipynb**: counts the number of each type of particle available (for now: electrons, gammas and alpha particles)
- **plot_particles.ipynb**: plots of some example of particles. the plots show both energy and noise separately. 

inside of counting_particles, there are available two python scripts:
- **crop_images.ipynb**: crops all energy images and moves them to a new directory.
- **dividing_particles.ipynb**: creates a directory for each type of particle and fills them with the data corresponding to each type of particle

inside of dataset_partition, there is available one python script:
- **creating_directories.ipynb**: slipts date into three dataset (train, validation, test)

inside of electrons_vs_noise, we can find three files:
- **eVSn.npz**: contains the electron energy and the noise stored separately
- **preparing_data_eVSn.ipynb**: notebook that prepares the npz file mentioned from the cropped images
- **electron_vs_noise.ipynb**: notebook where the convolutional neural network is built in order to classify as electron or noise
