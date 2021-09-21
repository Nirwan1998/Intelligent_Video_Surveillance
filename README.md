# Intelligent_Video_Surveillance
Deep Learning surveillance project

A spatio temporal autoencoder, which is based on a 3D convolution network. The encoder part extracts the spatial and temporal information, and then the decoder reconstructs the frames. The abnormal events are identified by computing the reconstruction loss using Euclidean distance between original and reconstructed batch.

Dataset used is the UCSD Pedestrian Dataset
*The folders Peds1 and Peds2 contain the individual frames of each clip in TIFF format.

*Peds1 contains 34 training video samples and 36 testing video samples. 

*Peds2 contains 16 training video samples and 12 testing video samples. All testing samples are associated with a manually-collected frame-level abnormal events annotation ground truth list (in the .m file).
   
*The training clips in both sets contain ONLY NORMAL FRAMES. 

*Each of the testing clips contain AT LEAST SOME ANOMALOUS FRAMES. 
A frame-level annotation of abnormal events is provided in the ground truth list under the test folder (in the form of a MATLAB .m file). The field 'gt_frame' indicates frames that contain abnormal events.

*10 test clips from the Peds1 set and 12 from Ped2 are also provided with PIXEL LEVEL GROUNDTRUTH MASKS.
These masks are labeled "Test004_gt", "Test014_gt", "Test018_gt" etc. in the Peds1 folder. 
(There is also full pixel level annotation on Ped1 for all 36 testing videos available at http://hci.iwr.uni-heidelberg.de/COMPVIS/research/abnormality)

*Citing:
	Anomaly Detection in Crowded Scenes.
	V. Mahadevan, W. Li, V. Bhalodia and N. Vasconcelos.
	In Proc. IEEE Conference on Computer Vision and Pattern Recognition (CVPR), 
	San Francisco, CA, 2010
