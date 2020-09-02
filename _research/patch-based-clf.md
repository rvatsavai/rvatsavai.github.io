---
title: "Complex Object Classification"
collection: research
type: "Research on identifying complex objects, multiple instance learning, ..."
permalink: /research/patch-based-clf
location: "ORNL and NCSU"
---

Research on identifying complex objects, multiple instance learning, ...

<ul>
  <li>Easy availability of very high-resolution (VHR) satellite imagery in the past decade has opened up newer applications 
    such as buiding detection, urban neighborhood classification, plantation counting and mapping, etc. However, traditional pixel
    based (single instance) classificaiton schemes proven to be inadequate as the size of objects are much bigger than the
    individual (or first/second order neighborhood) pixels. In addition to individual object (e.g., building) recognition,
    one can expoloit the much bigger spatial context (small image patch) to recognize complex facilities, such as, energy
    infrastructure (thermal, nuclear power plants) and urban neighborhoods (e.g., formal vs. informal settlements). We developed
    three classes of algorithms that exploit spatial context in VHR image classification. 
    In the first thread of research, we developed several novel image features
    that exploit spatial, structural, and contextual properties, and used them in machine learning models. In second thread of research,
    spatial context is exploited via image segmentation and object based neighborhood classification. Finally, we developed a novel
    multiple instance learning algorithm that solves limitations with image segmentation and single instance classification. Our algorithm,
    Gaussian Multiple Instance Learning (GMIL) shown to be not only accurate in complex object classification, but also very efficient
    as compared to the other state of the art single instance and multiple instance learning algorithms. Inaddtion, these algorithms
    are parallized on heterogenous architectures at Oak Ridge, that allowed utilization of patch based urban neighborhood classification
    in global settlement mapping and high-resolution population distribution estimates. This work is not only in practical use, but also
    published in major conferences like ACM SIGKDD and IEEE JSTARS. This work is also resulted in a US patent.
  </li>
  <li>. 
    <ul>
      <li>Vatsavai, Ranga Raju, Graesser, Jordan B., and Bhaduri, Budhendra L. Model for mapping settlements. 
        United States: Patent Publication Number: 20150055820, 2016.</li>
      <li>Manu Sethi, Yupeng Yan, Anand Rangarajan, Ranga Raju Vatsavai, Sanjay Ranka: 
        Scalable Machine Learning Approaches for Neighborhood Classification Using Very High Resolution Remote Sensing Imagery. ACM KDD 2015: 2069-2078</li>
      <li>Ranga Raju Vatsavai: Gaussian multiple instance learning approach for mapping the slums of the world using 
        very high resolution imagery. ACM KDD 2013: 1419-1426</li>
       <li>Jordan Graesser, Anil M. Cheriyadat, Ranga Raju Vatsavai, Varun Chandola, Jordan Long, Eddie A. Bright: 
        Image Based Characterization of Formal and Informal Neighborhoods in an Urban Landscape. IEEE J. Sel. Top. Appl. Earth Obs. 
        Remote. Sens. 5(4): 1164-1176 (2012)</li>       
    </ul>
  </li>
  </ul>
