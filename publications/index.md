---
layout: postnew
title: publications
<!-- in-nav: true -->
weight: 3
---

<div class="container">
    
    <div id="pubs">
    <div class="pubwrap">
      <div class="row">
        <div class="col-md-6">
          <div class="pubimg">
            <img src="http://cs.stanford.edu/people/karpathy/densecap.png">
          </div>
        </div>
        <div class="col-md-6">
          <div class="pub">
            <div class="pubt">DenseCap: Fully Convolutional Localization Networks for Dense Captioning</div>
            <div class="pubd">Efficiently identify and caption all the things in an image with a single forward pass of a network. Our model is fully differentiable and trained end-to-end without any pipelines. The model is also very efficient (processes a 720x600 image in only 240ms), and evaluation on a large-scale dataset of 94,000 images and 4,100,000 region captions shows that it outperforms baselines based on previous approaches.</div>
            <div class="puba">Justin Johnson*, Andrej Karpathy*, Li Fei-Fei</div>
            <div class="pubv">CVPR 2016 (Oral)</div>
            <div class="publ">
              <ul>
                <li><a href="densecap">Project</a></li>
                <li><a href="densecap.pdf">PDF</a></li>
                <li><a href="https://github.com/jcjohnson/densecap">Code (Github)</a></li>
              </ul>
            </div>
          </div>
        </div>
      </div>
      <div class="row">
        <img src="http://cs.stanford.edu/people/karpathy/densecap_more.jpg" style="max-width:100%; margin-top:30px;">
      </div>
    </div>

    <div class="pubwrap">
      <div class="row">
        <div class="col-md-6">
          <div class="pubimg">
            <img src="http://cs.stanford.edu/people/karpathy/rnn/icon.jpg">
          </div>
        </div>
        <div class="col-md-6">
          <div class="pub">
            <div class="pubt">Visualizing and Understanding Recurrent Networks</div>
            <div class="pubd">We study both qualitatively and quantitatively
              the performance improvements of Recurrent Networks in Language Modeling tasks compared to finite-horizon models. Our analysis sheds light on the source of improvements
              , and identifies areas for further potential gains. Among some fun results we find LSTM cells that keep track of long-range dependencies such as line lengths, quotes and brackets.</div>
            <div class="puba">Andrej Karpathy*, Justin Johnson*, Li Fei-Fei</div>
            <div class="pubv">ICLR 2016 Workshop</div>
            <div class="publ">
              <ul>
                <li><a href="http://arxiv.org/abs/1506.02078">PDF</a></li>
                <li><a href="http://github.com/karpathy/char-rnn">Code (char-rnn)</a></li>
                <li><a href="http://karpathy.github.io/2015/05/21/rnn-effectiveness/">Blog Post</a></li>
              </ul>
            </div>
          </div>
        </div>
      </div>
    </div>
    
    <div class="pubwrap">
        <div class="col-md-6">
          <div class="pubimg">
          <img src="http://cs.stanford.edu/people/karpathy/rnn7.png">
          </div>
        </div>
        <div class="col-md-6">
          <div class="pub">
            <div class="pubt">Deep Visual-Semantic Alignments for Generating Image Descriptions</div>
            <div class="pubd">We present a model that generates natural language descriptions of full images and their regions. For generating sentences about a given image region we describe a Multimodal Recurrent Neural Network architecture. For inferring the latent alignments between segments of sentences and regions of images we describe a model based on a novel combination of Convolutional Neural Networks over image regions, bidirectional Recurrent Neural Networks over sentences, and a structured objective that aligns the two modalities through a multimodal embedding. This work was also featured in a recent <a href="http://www.nytimes.com/2014/11/18/science/researchers-announce-breakthrough-in-content-recognition-software.html">New York Times article</a>.</div>
            <div class="puba">Andrej Karpathy, Li Fei-Fei</div>
            <div class="pubv">CVPR 2015 (Oral)</div>
            <div class="publ">
              <ul>
                <li><a href="cvpr2015.pdf">PDF</a></li>
                <li><a href="http://cs.stanford.edu/people/karpathy/deepimagesent/">Project</a></li>
                <li><a href="https://github.com/karpathy/neuraltalk2">Code (Github)</a></li>
                <li><a href="http://cs.stanford.edu/people/karpathy/deepimagesent/rankingdemo">Retrieval demo</a></li>
                <li><a href="http://techtalks.tv/talks/deep-visual-semantic-alignments-for-generating-image-descriptions/61593/">Presentation</a></li>
              </ul>
            </div>
          </div>
        </div>
    </div>
    </div>

    <div class="pubwrap">
      <div class="row">
        <div class="col-md-6">
          <div class="pubimg">
          <img src="http://cs.stanford.edu/people/karpathy/mosaic_sm.jpg">
          </div>
        </div>
        <div class="col-md-6">
          <div class="pub">
            <div class="pubt">ImageNet Large Scale Visual Recognition Challenge</div>
            <div class="pubd">Everything you wanted to know about ILSVRC: data collection, results, trends, current computer vision accuracy, even a stab at computer vision vs. human vision accuracy -- all here! My own contribution to this work were the <a href="http://karpathy.github.io/2014/09/02/what-i-learned-from-competing-against-a-convnet-on-imagenet/">human accuracy evaluation experiments</a>.
            </div>
            <div class="puba">Olga Russakovsky, Jia Deng, Hao Su, Jonathan Krause, Sanjeev Satheesh, Sean Ma, Zhiheng Huang, Andrej Karpathy, Aditya Khosla, Michael Bernstein, Alexander C. Berg, Li Fei-Fei</div>
            <div class="pubv">IJCV 2015</div>
            <div class="publ">
              <ul>
                <li><a href="http://arxiv.org/abs/1409.0575">PDF</a></li>
                <li><a href="http://karpathy.github.io/2014/09/02/what-i-learned-from-competing-against-a-convnet-on-imagenet/">Blog Post</a></li>
              </ul>
            </div>
          </div>
        </div>
      </div>
    </div>

    <div class="pubwrap">
      <div class="row">
        <div class="col-md-6">
          <div class="pubimg">
          <img src="http://cs.stanford.edu/people/karpathy/img/fragimg3.png">
          </div>
        </div>
        <div class="col-md-6">
          <div class="pub">
            <div class="pubt">Deep Fragment Embeddings for Bidirectional Image-Sentence Mapping</div>
            <div class="pubd">We train a multi-modal embedding to associate fragments of images (objects) and sentences (noun and verb phrases) with a structured, max-margin objective. Our model enables efficient and interpretible retrieval of images from sentence descriptions (and vice versa).</div>
            <div class="puba">Andrej Karpathy, Armand Joulin, Li Fei-Fei</div>
            <div class="pubv">NIPS 2014</div>
            <div class="publ">
              <ul>
                <li><a href="nips2014.pdf">PDF</a></li>
                <li><a href="nips2014_supp.pdf">Supplemental</a></li>
                <li><a href="defrag/index.html">Code</a></li>
                <li><a href="http://cs.stanford.edu/people/karpathy/defragvis/">Web Demo of Results</a></li>
              </ul>
            </div>
          </div>
        </div>
      </div>
    </div>

    <div class="pubwrap">
      <div class="row">
        <div class="col-md-6">
          <div class="pubimg">
            <img src="http://cs.stanford.edu/people/karpathy/img/videonets.png">
          </div>
        </div>
        <div class="col-md-6">
          <div class="pub">
            <div class="pubt">Large-Scale Video Classification with Convolutional Neural Networks</div>
            <div class="pubd">We introduce Sports-1M: a dataset of 1.1 million YouTube videos with 487 classes of Sport. This dataset allowed us to train large Convolutional Neural Networks that learn spatio-temporal features from video rather than single, static images.</div>
            <div class="puba">Andrej Karpathy, George Toderici, Sanketh Shetty, Thomas Leung, Rahul Sukthankar, Li Fei-Fei</div>
            <div class="pubv">CVPR 2014 (Oral)</div>
            <div class="publ">
              <ul>
                <li><a href="http://cs.stanford.edu/people/karpathy/deepvideo/">Project</a></li>
                <li><a href="http://cs.stanford.edu/people/karpathy/deepvideo/deepvideo_cvpr2014.pdf">PDF</a></li>
              </ul>
            </div>
          </div>
        </div>
      </div>
    </div>

    <div class="pubwrap">
      <div class="row">
        <div class="col-md-6">
          <div class="pubimg">
            <img src="http://cs.stanford.edu/people/karpathy/img/rnn.png">
          </div>
        </div>
        <div class="col-md-6">
          <div class="pub">
            <div class="pubt">Grounded Compositional Semantics for Finding and Describing Images with Sentences</div>
            <div class="pubd"> Our model learns to associate images and sentences in a common 

              We use a Recursive Neural Network to compute representation for sentences and a Convolutional Neural Network for images. We then learn a model that associates images and sentences through a structured, max-margin objective. </div>
            <div class="puba">Richard Socher, Andrej Karpathy, Quoc V. Le, Christopher D. Manning, Andrew Y. Ng</div>
            <div class="pubv">TACL 2013</div>
            <div class="publ">
              <ul>
                <li><a href="http://nlp.stanford.edu/~socherr/SocherKarpathyLeManningNg_TACL2013.pdf">PDF</a></li>
              </ul>
            </div>
          </div>
        </div>
      </div>
    </div>

    <div class="pubwrap">
      <div class="row">
        <div class="col-md-6">
          <div class="pubimg">
            <img src="http://cs.stanford.edu/people/karpathy/img/discovernet.png">
          </div>
        </div>
        <div class="col-md-6">
          <div class="pub">
            <div class="pubt">Emergence of Object-Selective Features in Unsupervised Feature Learning</div>
            <div class="pubd">
              We introduce an unsupervised feature learning algorithm that is trained explicitly with k-means for simple cells and a form of agglomerative clustering for complex cells. When trained on a large dataset of YouTube frames, the algorithm automatically discovers semantic concepts, such as faces.
            </div>
            <div class="puba">Adam Coates, Andrej Karpathy, Andrew Ng</div>
            <div class="pubv">NIPS 2012</div>
            <div class="publ">
              <ul>
                <li><a href="http://cs.stanford.edu/people/karpathy/nips2012.pdf">PDF</a></li>
              </ul>
            </div>
          </div>
        </div>
      </div>
    </div>

    <div class="pubwrap" style="border-bottom: none; padding-bottom:0px; margin-bottom:30px;">
      <div class="row">
        <div class="col-md-6">
          <div class="pubimg">
            <img src="http://cs.stanford.edu/people/karpathy/img/quadruped.png">
          </div>
        </div>
        <div class="col-md-6">
          <div class="pub">
            <div class="pubt">Locomotion Skills for Simulated Quadrupeds</div>
            <div class="pubd">We develop an integrated set of gaits and skills for a physics-based simulation of a quadruped. The controllers use a representation based on gait graphs, a dual leg frame model, a flexible spine model, and the extensive use of internal virtual forces applied via the Jacobian transpose.</div>
            <div class="puba">Stelian Coros, Andrej Karpathy, Benjamin Jones, Lionel Reveret, Michiel van de Panne</div>
            <div class="pubv">SIGGRAPH 2011</div>
            <div class="publ">
              <ul>
                <li><a href="http://www.cs.ubc.ca/~van/papers/2011-TOG-quadruped/index.html">Project</a></li>
              </ul>
            </div>
          </div>
        </div>
      </div>
    </div>

  </div>