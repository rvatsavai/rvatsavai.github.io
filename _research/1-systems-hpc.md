---
title: "Systems Research (HPC/ML)"
collection: research
permalink: /research/1-systems-hpc
---

Research on scaling machine learning algorithms, graph databases, geosimulations, in-situ analytics, ...

<ul>
  <li><span style="color:red">Scaling Machine Learning Algorithms</span>
     <ul>
      <li>Gaussian Process (GP) Learning: GP based approaches are increasingly being used as a kernel machine learning tool for 
        nonparametric regression and classification. We developed several novel algorithms based on GP learning for classification, 
        change detection and anomaly detection. Despite great advantages of GP in various machine learning tasks, in particular 
        for spatial and temporal data, its wide adaption is limited due
        to it's high computational complexity, O(t<sup>3</sup>), and memory footprint, O(t<sup>2</sup>), where t is the length of time 
        series. In applications like monitoring crop biomass at regional scales, one has to deal with billions of time series, and the 
        solution requires computation of covariance matrix  and its inversion for each time series. To overcome these limitations, we 
        chose a exponential covariance function that captures not only the periodic nature of crop growth (phenology) and but also 
        efficient as the resulting covariance is a Toeplitz matrix. Our new solution, GPChange, has reduced complexity to O(t<sup>2</sup>)
        and memory to O(t). In addition, we developed mixed parallel algorithms to take advantage of heterogeneous 
        compute clusters at Oak Ridge leadership computing facility. Our experiments showed significant reduction in computing time 
        from days to seconds compared to the standard Cholesky decomposition based GP learning on a 128 node SGI Altrix ICE 8200 cluster. 
        This solution was operationalized at Oak Ridge for regional scale continuous biomass monitoring using MODIS satellite based daily 
        NDVI time series. In addition to publishing several papers in leading conferences and journals, the project won 
        the <span style="color:red">ORNL Lab Director's best LDRD project award </span> for the year 2010.
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
      <li>Geosimulations are widely used in urban growth modeling, environmental studies, disease spread modeling,
        traffic modeling, and land-use and land-cover changes. Geosimulations are increasingly becoming sophisticated,
        however computational complexity has also increasing along with increase in spatial/temporal extents and final resolutions.
        To address these computational and I/O challenges, we developed various parallelization strategies for scaling cellular automation 
        based FUTURES model in distributed computing environment. In particular, we developed intelligent strategies for data
        partitioning, task scheduling, and task synchronization. These strategies have resulted in a highly scalable 
        <span style="color:red">pFUTURES</span> model, which made it possible to study urban simulations for large spatial and temporal extents at
        a finer spatial resolution than previously reported in the literature. In addition, we developed an adaptive
        mesh refinement strategy, <span style="color:red"> FUTURES-AMR</span>, that further reduced computation 
          and memory requirements for large scale simulations. 
        Typical data parallel approaches in geosimulations use static partitioning strategy along with load-balancing, 
        however in many practical situations some tiles (data partitions) may require the simulations to run at finer 
        resolutions than the other tiles (e.g., to account for important and critical events such as flooding). To account
        for such scenarios, we developed a novel provisioning system, <span style="color:red">FUTURES-DPE</span>, 
          that dynamically allocates additional computing 
        resources to the required tiles at run-time. This extension along with our computational steering work, 
        for the first time allowed geosimulation modelers to explore
        what-if scenarios on-the-fly. The <span style="color:red"> FUTURES-AMR</span> work is nominated for best 
        paper award at the top ranking biennial GIScience 2018 conference.
        
   <ul>
          <li>Ashwin Shashidharan, Ranga Raju Vatsavai, Ross K. Meentemeyer: "FUTURES-DPE: 
            towards dynamic provisioning and execution of geosimulations in HPC environments." 
            The ACM SIGSPATIAL International Conference on Advances in Geographic Information Systems (SIGSPATIAL/GIS) 2018: 464-467 </li>
          <li>Ashwin Shashidharan, Ranga Raju Vatsavai, Derek B. van Berkel, Ross K. Meentemeyer: "FUTURES-AMR: 
            Towards an Adaptive Mesh Refinement Framework for Geosimulations." The
            International Conference on Geographic Information Science (GIScience) 2018: 16:1-16:15 
            (<span style="color:red">nonimanted for the best paper</span>)</li>
          <li>Qiang Zhang, Ranga Raju Vatsavai, Ashwin Shashidharan, Derek B. van Berkel: Agent based urban growth 
            modeling framework on Apache Spark. BigSpatial@SIGSPATIAL 2016: 50-59 </li>
          <li>Ashwin Shashidharan, Derek B. van Berkel, Ranga Raju Vatsavai, Ross K. Meentemeyer: "pFUTURES: 
            A Parallel Framework for Cellular Automaton Based Urban Growth Models." The 
            International Conference on Geographic Information Science (GIScience) 2016: 163-177 </li>
     </ul>        
      </li>        
     </ul> 
  </li>  
  <li><span style="color:red">In Situ Analytics:</span>
     <ul>
       <li> Hi-resolution simulations on exascale supercomputers are producing petabytes of data. Storing
         and retriving such large dataset for analytics is a challenging task. In situ analytics aims at
         on-the-fly data compression and summarization before the data hits secondary storage. 
         Summarization and compression at current and future scales requires a framework for 
         developing and benchmarking algorithms. We developed a novel framework by integrating existing, 
         production-ready projects in VTK and demonstrated scaling results of two particular algorithms 
         that serve as exemplars for summarization: a wavelet-based data reduction filter and a generator 
         for creating image-like databases of extracted features (isocontours in this case). Both these
         solutions support browser-based, post-hoc, interactive visualization of the summary for decision-making. 
         We also demonstrated weak-scaling on a distributed multi-GPU system.
         <ul>
           <li>David C. Thompson, Sébastien Jourdain, Andrew C. Bauer, Berk Geveci, Robert Maynard, 
             Ranga Raju Vatsavai, Patrick O'Leary: In Situ Summarization with VTK-m. ISAV@SC 2017: 32-36
           </li>
         </ul>
         
       </li>
    </ul>
  </li>
</ul>
