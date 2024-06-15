# test-multiclass-segmentation
This repository contains 

# Task:
Within **4 hours** please attempt to build, train and test a deep learning model that can segment Sentinel-2 image tiles into a 6-class land cover map. Specifically please do the following:
1. train your model only on images and masks in the *tra_scene/* and *tra_truth/* directory.
2. evaluate your model only on images and masks in the *val_scene/* and *tra_truth/* directory
3. during evaluation, please use the [jaccard_score](https://scikit-learn.org/stable/modules/generated/sklearn.metrics.jaccard_score.html) function. Calculate it per class, and the average score across all classes.
4. use your best model to make inference over the first image in the *val_scene/* directory. Plot the resulting segmentation alongside the true land cover mask.yhj
5. send an email to roald.vang@nina.no as soon as you are finished with the following:
    - your code
    - a printout of the highest jaccard_score (averaged over all classes)
    - a jpeg figure showing the resulting segmentation (point 4 above)

The Sentinel-2 image tiles and land cover masks have been made available in this repository along with a short Python notebook to get you started. 

Please send your code to roald.vang@nina.no as soon as you are finished. We will calculate the time taken as the difference between when you send the email and when you opened the Microsoft Forms link. If you are over-time, this will count against you in the evaluation of your work. So do as much as you can witin 4 hours and don't stress if you cannot complete all the points listed above!

### Repository Structure

```bash
test-multiclass-segmentation/
├── dset-s2-grunnkart/
│   ├── tra_scene
|   ├── tra_truth
|   ├── val_scene
│   └── val_truth
├── multiclass_segmentation.ipynb
└── README.md
