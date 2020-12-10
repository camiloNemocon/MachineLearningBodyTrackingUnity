# MachineLearningBodyTrackingUnity
This proyect is a system body tracking using Machine Learning in Unity  through Barracuda to move avatar 3d model


This proyect is a system body tracking using Machine Learning in Unity 
through Barracuda, using a training model (https://digital-standard.com/threedpose/models/Resnet34_3inputs_448x448_20200609.onnx) in ONX to recognice the body from a video or webcam to transfer the joint position to a model 3d.

This project is based on the "ThreeDPoseUnityBarracuda”, developed by Hinori (https://github.com/digital-standard/ThreeDPoseUnityBarracuda).

In this project you can add easly a 3d model, following the next steps:

1. Download file .onnx model: https://drive.google.com/file/d/1yviZ3Mze8MNf2TYpYA12_p66YOzfkmvY/view?usp=sharing
2. Copy the file .onnx on folder:  BarracudaBodyTracking\Assets\Scripts\Model
3. Open SampleScene from Scenes folder
4. Unity -> Play

If you like to change model 3d Avatar you need:
1. Add 3d model with rigging (bones for al the body include hands finger bones) in Unity project.
2. Modify the features of the rigging, using the tool Rig/Configure of Unity.
3. The bones are automatically associated with the components of the 3d model.
4. Put the 3d model on the scene and add the script VNectModel to the 3d model.
5. On BarracudaRunner Object in inspector select the new 3d model on VNectModel section.
