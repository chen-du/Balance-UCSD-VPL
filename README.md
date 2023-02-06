# Balance-UCSD-VPL
 
This dataset contains 11,028 3D body landmark sequences and corresponding center of pressure measurements for balance-related movement video clips. Each video clip includes 120 frames of 3D body landmarks and their affiliated center of pressure position.

This dataset includes data from 21 healthy adults. During the collection phase, each subject stood on the force plate with no shoes using 1) feet side-by-side and 2) feet-in-tandem (i.e., heel-to-toe) postures. We instructed subjects to perform random movements, e.g., from rigid standing to body swaying, involving the trunk, arms, hands, or bending knees. The only specified requirement was not to move the feet; we provided no specific instructions about the action patterns.

The video was collected by two calibrated RGB cameras using a resolution of 640 x 480 pixels at 30 fps, while the center of pressure was recorded at 60 Hz using a force plate. Please refer to the following publications for more details.

## File format
BodyLandMark.npy contains the 3D body landmarks in meter (m); the shape of the data is 11028 (clips) * 120 (frames) * 25 (joints) * 3 (dimensions)

CenterOfPressure.npy contains the corresponding center of pressure measurements (x, y) in centimeters (cm) for each video clip; the shape of the data is 11028 (clips) * 120 (frames) * 2 (dimensions)

Split.npy contains the data split for each clip in the mixed-subject evaluation, 0 for the training set, 1 for the validation set, 2 for the testing set.

## Citation

If you make use of the dataset, please consider citing the following references in any publications:

Chen Du, Sarah Graham, Colin Depp, and Truong Nguyen. "Multi-Task Center-of-Pressure Metrics Estimation With Graph Convolutional Network." IEEE Transactions on Multimedia 24 (2021): 2018-2033.

Chen Du, Sarah Graham, Shiwei Jin, Colin Depp, and Truong Nguyen. "Multi-task center-of-pressure metrics estimation from skeleton using graph convolutional network." In ICASSP 2020-2020 IEEE International Conference on Acoustics, Speech and Signal Processing (ICASSP), pp. 2313-2317. IEEE, 2020.


## Contact
If you have any questions, please contact c9du@ucsd.edu
