---
title: "Anomaly Detection (Spatiotemporal, Videos)"
collection: research
type: "Research on identifying anomalous patterns in climate change data, videos, ..."
permalink: /research/4-anomalies
location: "ORNL and NCSU"
---

Research on identifying anomalous patterns in climate change data, videos, ...

<ul>
  <li><span style="color:red">Spatiotemporal Anomalies:</span> 
    Finding anomalous regions in spatiotemporal data is a challenging task. For example, the collective 
    and contextual nature of anomalies (e.g., heat waves) coupled 
    with the real-valued, seasonal, multimodal, highly correlated, and gridded nature of spatiotemporal (climate variable)
    observations poses a multitude of challenges. Existing anomaly detection methods have limitations in 
    the specific setting of real-valued areal spatiotemporal data. To address these challenges, we develop a novel method 
    for extreme event detection in meteorological datasets that follows from well known distribution-based 
    anomaly detection approaches. This method models spatial and temporal correlations explicitly through a 
    piecewise parametric assumption and generalizes the Mahalanobis distance across distributions of different 
    dimensionalities. This method is shown to be very effective in mining contiguous spatiotemporal anomalous regions 
    from meteorological fields and shown to be accurate than current standard approaches in climatology. We also developed
    an efficient and parallel anaomaly detection technique based on Gaussian Process (GP) regression. 
    <ul>
      <li>Bharathkumar Ramachandra, Benjamin Dutton, Ranga Raju Vatsavai: Anomalous cluster 
        detection in spatiotemporal meteorological fields. Statistical Analysis and Data 
        Mining 12(2): 88-100 (2019)</li>
      <li>Krishna Karthik Gadiraju, Bharathkumar Ramachandra, Ashwin Shashidharan, Benjamin Dutton, 
        Ranga Raju Vatsavai: Scalable Data Parallel Approaches to Anomaly Detection in Climate Data 
        using Gaussian Processes. ICMLA 2019:</li>
    </ul>
  </li>

  <li><span style="color:red">Video Anomalies:</span>
  Our current research is focused on a closely related topic of anomaly detection in videos. Video anomaly detection 
  is the task of localizing anomalies in space and/or time in a video, where anomalies are simply activities that are 
  out of the ordinary. Most previous methods have limitations that can be attributed to one or more of the following, 
  which served as the motivation for our research: (1) The features used in many methods are hand-crafted, (2) Almost 
  every method requires a computationally expensive model building phase requiring expert knowledge which may not be 
  practical for real applications, and (3) Many previous works focus on detecting only specific deviations from normality 
  as anomalous. We did a comprehensive survey of this field, and a survey article is under (2nd round) review at IEEE TPAMI.
  To overcome, some of these limitations, we devloped a novel method that uses a Siamese convolutional neural network (CNN) 
  to learn a distance function between a pair of video patches (spatiotemporal regions of video). The learned distance 
  function, which is not specific to the target video, is used to measure the distance between each video patch in the 
  testing video and the video patches found in normal training video. Experiments on 3 challenging target benchmark datasets
  showed that our approach either surpasses or performs comparably to current state-of-the-art methods. 
    <ul>
      <li>Bharathkumar Ramachandra, Michael J. Jones, Ranga Raju Vatsavai: A Survey of Single-Scene Video 
        Anomaly Detection. CoRR abs/2004.05993 (2020) (Under review at IEEE TPAMI)</li>
      <li>Bharathkumar Ramachandra, Michael J. Jones, Ranga Raju Vatsavai: Learning a distance function 
        with a Siamese network to localize anomalies in videos. IEEE Winter Conference on Applications of 
        Computer Vision, WACV 2020: 2587-2596</li>       
    </ul>
  </li>
</ul>
