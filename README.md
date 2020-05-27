# TFM
scripts and data examples of my master's thesis

inside of counting_particles, there are available two python scripts:
- **num_particles.ipynb**: counts the number of each type of particle available (for now: electrons, gammas and alpha particles)
- **plot_particles.ipynb**: plots of some example of particles. the plots show both energy and noise separately. 

inside of preprocessing, there are available two python scripts:
- **crop_images.ipynb**: crops all energy and noise images and moves them to a new directory.

inside of dataset_partition, there is available one python script:
- **creating_directories.ipynb**: slipts date into three dataset (train, validation, test)

inside of electrons_vs_noise, we can find six files:
- **eVSn_1.npz**: contains the electron energy and the noise stored separately
- **preparing_data_eVSn.ipynb**: notebook that prepares the npz file just mentioned from the cropped images
- **electron_vs_noise.ipynb**: notebook where convolutional neural networks are built in order to classify as electron or noise
- **add_noise_to_e.ipynb**: notebook where the noise is added to the energy signal to create a npz file called eVSn_noisy1
- **eVSn_noisy1.npz**: contains the electron energy+noise and the noise stored separately
- **e_noisy_vs_noise.ipynb**: notebook where convolutional neural networks are built in order to classify as electron or noise, but in this case, the image of the electron includes also noise

inside of electrons_vs_muons, we can find eight files:
- **less_data**: folder contaning first round of data. There are two files, one with the training and validation data and the other one left, containig the testing data. The training dataset has been over/undersampled.
- **more_data**: folder contaning first round of data. There are three files, one with the traning, another with validation data and the last one, containig the testing data. The training dataset has been over/undersampled. The training dataset has been over/undersampled.
- **models**: models created with the data stored in the more_data folder.
- **balancing_data.ipynb**: this notebook contains the code to balance our dataset and shows how we got the npz files mentioned.
- **add_noise_balacing.ipynb**: this notebooks adds noise to the energy of the particles and balances the dataset.
- **data_eVSmu2.ipynb**: pads/crops the energy/noise files of electrons and muons with the data stored in the more_data folder.
- **data_generator.ipynb**: notebook to create the batches that will be used for the training, validation and testing of the model.
- **e_VS_mu.ipynb**: notebook where convolutional neural networks are built in order to classify as electron or muon with the date inside less_data
- **e_VS_mu.ipynb**: notebook where convolutional neural networks are built in order to classify as electron or muon with the date inside more_data
-**standardizing_data(npz).ipynb**: standardizes the data before feeding it to the models

inside of electrons_vs_muons_vs_noise, we can find four files:
- **models**: models created with the data stored in the more_data folder.
- **modelsN**: models created with the data stored in the more_data folder, but this time with noise added to the particles energy.
- **add_noise.ipynb**: adds noise to the energy signals of electrons and muons.
- **data_generator.ipynb**: notebook to create the batches that will be used for the training, validation and testing of the model.
- **data_generator_noisy.ipynb**: notebook to create the batches that will be used for the training, validation and testing of the model in the case where the electrons and muons have noise in their energy signals.
- **data_eVSmuVSn.ipynb**: pads/crops the energy/noise files of electrons and muons with the data stored in the more_data folder.
- **preparing_noise.ipynb**: creates a new class, the noise class, from the noise stored in the electron files.
- **e_VS_mu_VS_n2.ipynb**: notebook where convolutional neural networks are built in order to classify as electron, muon or noise
- **e_VS_mu_VS_n2N.ipynb**: notebook where convolutional neural networks are built in order to classify as electron, muon or noise but this time with noise added to the particles energy.
- **standardizing_data(npz).ipynb**: standardizes the data before feeding it to the models
- **standardizing_data(npz)N.ipynb**: standardizes the data before feeding it to the models but this time with noise added to the particles energy.
