---
title: "Systems Research (HPC)"
collection: research
permalink: /research/systems-hpc
---

Research on scaling machine learning algorithms, graph databases, geosimulations ...

<ul>
  <li><span style="color:red">Scaling Machine Learning Algorithms</span>
     <ul>
      <li>Gaussin Process (GP) Learning: GP based approaches are increasingly being used as a kernel machine learning tool for 
        nonparametric regression and classification. We developed several novel algorithms based on GP learning for classification, 
        change detection and anomaly detection. Despite great advantages of GP in various machine learning tasks, its wide adaption is limited due
        to it's high computational complexity, O(t<sup>3</sup>), and memory footprint, O(t<sup>2</sup>), where t is the lenght of time 
        series. In applications like monitoring crop biomass at regional scales, one has to deal with billions of time series, and the 
        solution requires computation of covariance matrix  and its inversion for each time series. To overcome these limitations, we 
        chose a exponential covariance function that captures not only the periodic nature of crop growth (phenology) and but also 
        efficient as the resulting covariance is a Toeplitz matrix. Our new solution, GPChange, has reduced complexity to O(t<sup>2</sup>)
        and memory to O(t). In addition, we developed mixed parallel algorithms to take advantage of heterogeneous 
        compute clusters at Oak Ridge leardership computing facility. Our experiments showed significant reduction in computing time 
        from days to seconds compared to the standard Cholesky decomposition based GP learning on a 128 node SGI Altrix ICE 8200 cluster. 
        This solution was operationalized at Oak Ridge for regional scale continuous biomass monitoring using MODIS satellite based daily 
        NDVI time series. In addition to publishing several papers in leading conferences and journals, the project won ORNL Lab Director's
        best LDRD project for the year 2010.
        <ul>
          <li>Varun Chandola, Ranga Raju Vatsavai: A scalable gaussian process analysis algorithm for biomass monitoring. 
            Statistical Analysis and Data Mining 4(4): 430-445 (2011) </li>
          <li>Varun Chandola, Ranga Raju Vatsavai: A Gaussian Process Based Online Change Detection Algorithm for 
            Monitoring Periodic Time Series. SIAM Data Mining (SDM) 2011: 95-106 </li>
          <li>Varun Chandola, Ranga Raju Vatsavai: Scalable Time Series Change Detection for Biomass Monitoring 
            Using Gaussian Process. NASA Conference on Intelligent Data Understanding (CIDU) 2010: 69-82.
            (Selected as one of the <span style="color:red">six best papers at the NASA/CIDU</span> and 
            published in the special issue of Statistical Analysis and Data Mining Journal)</li>
        </ul>
      </li>        
     </ul> 
  </li>
  
  <li><span style="color:red">Scaling GeoSimulations:</span>
     <ul>
      <li>Gaussin Process Learning: 
      </li>        
     </ul> 
  </li>  
</ul>
