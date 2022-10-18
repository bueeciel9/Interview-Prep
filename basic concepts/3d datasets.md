KITTI is recorded in daytime on sunny days, without taking lighting and weather conditions into account, resulting a relative lower diversity compared with nuScenes and Waymo Open. Real dataset tends to suffer from class imbalance as it is true to life. According to our statistics in Table 3, 50% categories account for only 6.9% of total annotations, which clearly reflects a long-tail distribution on nuScenes.

KITTI:
3D detection and Bird’s Eye View (BEV) detection. 3D detection evaluates AP3DðR11 with a rotated IoU3D threshold of 0.7, 0.5, 0.5 for Car, Pedestrian and Cyclist accordingly. The principles of 3D detection largely holds true for BEV detection, except for the calculation of IoUBEV , which is calculated by projecting the bounding boxB3D from 3D pace into the ground plane.

NuScenes:
It is worth noting that mAP is calculated by a bird-eye-view center distance of thresholds ^0:5m; 1m; 2m; 4m rather than standard box-overlap.

Waymo:
Waymo Open leverages Interpolated APðR21 Metric and Average Precision weighted by Heading (APH) as its primary metric for evaluating detector F .X ; To compute AP, Waymo evaluates on 21 equally spaced recall levels 0; 1_20; 2_20; :::; 1 in Equation 2 with an IoU threshold of 0.7, 0.5 for vehicles, pedestrians respectively.


