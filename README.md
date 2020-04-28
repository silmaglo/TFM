# TFM
scripts and data examples of my master's thesis

inside of counting_particles, there are available two python scripts:
- **num_particles.ipynb**: counts the number of each type of particle available (for now: electrons, gammas and alpha particles)
- **plot_particles.ipynb**: plots of some example of particles. the plots show both energy and noise separately. 

inside of preprocessing, there are available two python scripts:
- **crop_images.ipynb**: crops all energy and noise images and moves them to a new directory.
- **dividing_particles.ipynb**: creates a directory for each type of particle and fills them with the data corresponding to each type of particle

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
- **eVSmu_tr1.npz** and **eVSmu_te1.npz**: both contain energy and the noise stored separately of muons and electrons, but the first filee constitutes the training dataset and the second one, the test data. The training dataset has been over/undersampled.
- **eVSmu_te2.npz**, **eVSmu_tr2.npz** and **eVSmu_va2.npz**: both contain energy and noise stored separetely of muons and electrons. The first one has the testing data, the second one the training and the last one, the validation data. The training dataset has been over/undersampled.
- **balancing_data.ipynb**: this notebook contains the code to balance our dataset and shows how we got the npz files mentioned.
- **data_eVSmu.ipynb**: selects the data of muons and electrons in specific directories.
- **e_VS_mu.ipynb**: notebook where convolutional neural networks are built in order to classify as electron or muon

inside of electrons_vs_muons_vs_noise, we can find four files:
- **data_eVSmuVSn.ipynb**: contains the electron/muon energy and the noise stored separately, and also the noise
- **add_noise_balacing.ipynb**: adds noise to the energy signals and balances the dataset so the three classes (electron, muon and noise) have the same number of samples
- **e_VS_mu_VS_n.ipynb**: notebook where convolutional neural networks are built in order to classify as electron, muon or noise
- **e_VS_mu_VS_n_noisy.ipynb**: notebook where convolutional neural networks are built in order to classify as electron, muon or noise, but in this case, the energy image includes also noise
- **eVSmuVSn_1.npz**: npz file with the data of electrons, muons and noise
- **eVSmuVSn_te1.npz** and **eVSmuVSn_tr1.npz**: both contain energy and the noise stored separately of muons and electrons, but the first filee constitutes the test data and the second one, the training data. The training dataset has been over/undersampled. We have three classes: electron, muon and noise.
- **eVSmuVSn_noisyte1.npz** and **eVSmuVSn_noisytr1.npz**: same as the files before but the energy images are noisy
