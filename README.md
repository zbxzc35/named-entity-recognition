#named-entity-recognition
=====================

Using both MITIE library and Convnet.

To run this code, you should have 
* OpenCV
* MITIE lib & dlib (new version can be found in [MITIE github](https://github.com/mit-nlp/MITIE))

##Compile & Run

* Download MITIE and install mitie models by running:
```
make MITIE-models
```
* put ```mitielib``` folder and ```dlib``` into ```named-entity-recognition``` folder
* put ```MITIE-models/english/total_word_feature_extractor.dat``` into ```./network``` folder

* Compile by running:
```
cmake .
make
```
* Run: 
```
./NER x
```
* where x is run mode:
  - 1: Train mitie
  - 2: Train convolutional neural networks
  - 3: Do named entity recognition using mitie
  - 4: Do named entity recognition using convolutional neural networks

##Structure and Algorithm
See [my tech-blog](http://eric-yuan.me/ner_1).

##TODO
...

##MITIE LICENSE
MITIE is licensed under the Boost Software License.

The MIT License (MIT)
------------------

Copyright (c) 2014 Xingdi (Eric) Yuan

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.