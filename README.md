# CS4371
Anomaly detection simulation using Isolation Forest, LOF, and adaptive autoencoders.


Contemporary Reference (Follow-up / Forward-Looking):
Mammeri, A., Zrelli, M. H., & Zhou, J. (2023).
"Collaborative perception-based anomaly detection for autonomous driving systems."
Journal of Network and Computer Applications.
https://doi.org/10.1016/j.jnca.2023.103699

This paper discusses advanced anomaly detection systems in CAVs that use collaborative perception—just like the CAD system your project is trying to replicate and expand upon. It explores how sharing sensor data (like LiDAR) across vehicles increases performance but also the attack surface, reinforcing the need for adaptive and memory-informed anomaly detection models like your final autoencoder version.

How Your Code Relates to These Works:
basic_detection_isoforest.py: Reflects the foundational concept of detecting anomalies using static models. The model has no memory or adaptation—mirroring the early, simpler anomaly detection models.

adaptive_detection_lof.py: An intermediate step. It has limited adaptation (remembers the last run), using Local Outlier Factor, which bridges simple and learning-based models.

adaptive_detection_autoencoder.py (non-adaptive): Trains once—akin to a student cramming before exams. Reflects many current machine learning deployments that struggle with generalization over time.

adaptive_detection_autoencoder.py (adaptive): This version retrains after each run and best simulates the CAD system from your paper. It’s the most advanced and forward-looking, aligning with current trends in adversarial-aware and real-time anomaly detection in smart vehicles.
