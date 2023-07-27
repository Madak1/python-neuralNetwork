# Dataset Description

**Dataset general overview**

This data set contains algae images captured by a color digital holographic microscope (DHM). DHM is a volumetric microscope, which captures a hologram from an entire sample volume, which is roughly 1mm x 1mm x 0.8mm. (As a comparison, one should capture 800 images with a traditional brightfield microscope to span over this large depth.) The hologram contains the aggregated information of the entire sample volume. With mathematical methods, one can calculate a focused image in any depth within the sample. Naturally, the images are corrupted with interference, twin images and other artifacts due to the applied coherent imaging technique, therefore the images are not as nice as traditional microscopic images.

The data base was generated on a way that samples were collected from different natural surface waters, and the samples were processed by the DHM. The DHM took the hologram images, found the individual algae on each hologram one after the other, made them sharp, and cut them. Then, the data base was hand selected (categorized) by biologists.

**Properties of the dataset**

- The dataset contains 6 classes based on the number of algae in a cluster and 2 additional classes which has debris and small particles instead of algae
- There are a relatively low number of samples ~3500 images total
- The train and the test set has similar - highly unbalanced - distribution

**Structure of the downloaded data set**

- The downloaded dataset contains 8 folders:
  - one for each class, containing the image samples of that class
  - the names of the folders are the names of the categories
  - a single folder called "db_chlorella_renamed_TEST", which contains all the testset images (no class label is provided)
- Finally, it has a .txt file called "sample_submission.txt" that contains an example of how your solution file should look like. Note that it should have as many rows as many samples there are in the testset.
