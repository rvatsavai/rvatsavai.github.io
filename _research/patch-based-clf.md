---
title: "Complex Object Classification"
collection: research
type: "Research on identifying complex objects, multiple instance learning, ..."
permalink: /research/patch-based-clf
location: "ORNL and NCSU"
---

Research on identifying complex objects, multiple instance learning, ...

<ul>
  <li>I made significant contributions to the change detection research through: (i) efficient modeling of crop phenology, 
    and (ii) efficient modeling of spatial context via image patches. Change detection using remote sensing time series poses 
    two challenges: (i) distinguishing between real changes (e.g., due to damages, change in crop-type from season to season) 
    from normal or expected changes (e.g., changes in green- ness over crop growing season, environmental effects), and 
    (ii) scalability (continental scale). I developed a novel biomass monitoring framework that consists of two key 
    components: change detection using Gaussian Process (GP) Learning, and change characterization using semi-supervised 
    learning. Through a well designed covariance matrix (Toeplitz) that efficiently captures crop phenology, our GP-based 
    change detection framework not only showed the improved accuracy (25% over Bayesian Online Change Detection), but also 
    reduced the computational complexity (time complexity from O(n3) to O(n2) and memory usage from O(n2) to O(n)). 
    In addition, efficient (mixed) parallel implementation has lead to the continental scale continuous monitoring 
    system using daily MODIS satellite image data. This work was well received (won “Directors Best R&D” award at annual 
    ORNL Lab Directed R&D project evaluations; selected as one of the six best papers at NASA CIDU Conference (2010) 
    it got invited to a special issue of Statistical Analysis and Data Mining Journal (4(4), 2011)). 
  </li>
  <li>In addition to the biomass monitoring (which is critical for food security), my research had also resulted 
    in a key capability for monitoring man-made critical infrastructures which allows comparing multi-sensor and 
    multi-resolution images which may not have been perfectly georegistered. Traditional remote sensing based change
    detection approaches compare individual (or first/second order neighborhood) pixels to idenfify changes. However,
    image to image and map to image registrations, through increasingly becoming accurate, contains errors (often by several
    pixels), as a result direct pixel-wise comparision is not accurate. In addition, often changes happen at a bigger spatial
    footprint than individual pixels. To overcome these limitations, we developed a novel and unique image patch-based 
    probabilistic change detection that shown to be not only accurate than traditional methods, but also allows 
    multi-resolution and multi-sensor data. The results were published in leading venues (Procedia Computer Science, 
    Vol. 9, 2012; Demo paper at ICDM 2012), and has been extensively used in several NGA, DOD, and DHS sponsored 
    projects at the ORNL. 
    <ul>
      <li>A. Karpatne, Z. Jiang, R. R. Vatsavai, S. Shekhar and V. Kumar, "Monitoring Land-Cover Changes: 
        A Machine-Learning Perspective," in IEEE Geoscience and Remote Sensing Magazine, vol. 4, no. 2, pp. 8-21, June 2016, doi: 10.1109/MGRS.2016.2528038.</li>
      <li>Clayton Connors, Ranga Raju Vatsavai: Semi-supervised deep generative models for change detection 
        in very high resolution imagery. IGARSS 2017: 1063-1066 </li>
      <li>Zexi Chen, Bharathkumar Ramachandra, Ranga Raju Vatsavai: Hierarchical change detection 
        framework for biomass monitoring. IGARSS 2017: 620-623 </li>
      <li>Zexi Chen, Ranga Raju Vatsavai, Bharathkumar Ramachandra, Qiang Zhang, Nagendra Singh, 
        Sreenivas Sukumar: Scalable nearest neighbor based hierarchical change detection framework for crop monitoring. 
        BigData 2016: 1309-1314 </li>
      <li>Ranga Raju Vatsavai: Rapid Damage eXplorer (RDX): A Probabilistic Framework for Learning Changes from 
        Bitemporal Images. IEEE International Conference on Data Mining (ICDM: Demo Paper) 2012: 906-909</li>
      <li>Ranga Raju Vatsavai, Jordan Graesser: Probabilistic Change Detection Framework for Analyzing 
        Settlement Dynamics Using Very High-resolution Satellite Imagery. ICCS 2012: 907-916</li>
      <li>Varun Chandola, Ranga Raju Vatsavai: A Gaussian Process Based Online Change Detection Algorithm for 
        Monitoring Periodic Time Series. SIAM Data Mining Conference (SDM 2011): 95-106 </li>
      <li>Varun Chandola, Ranga Raju Vatsavai: Scalable Time Series Change Detection for Biomass Monitoring 
            Using Gaussian Process. NASA Conference on Intelligent Data Understanding (CIDU) 2010: 69-82.
            (Selected as one of the <span style="color:red">six best papers at the NASA/CIDU</span> and 
            published in the special issue of Statistical Analysis and Data Mining Journal)</li>
    </ul>
  </li>
  </ul>
