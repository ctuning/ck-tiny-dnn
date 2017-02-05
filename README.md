Collective Knowledge repository for evaluating and optimising Tiny DNN

Introduction
============

We need to have easily customizable Tiny DNN builds 
via JSON API to be able to plug it to our framework 
for collaborative benchmarking and optimization of workloads 
across diverse inputs and hardware provided by volunteers 
(see [cKnowledge.org/ai](http://cKnowledge.org/ai), 
[live repo](http://cKnowledge.org/repo)
and papers [1](https://arxiv.org/abs/1506.06256), 
[2](https://scholar.google.com/citations?view_op=view_citation&hl=en&user=IwcnpkwAAAAJ&citation_for_view=IwcnpkwAAAAJ:maZDTaKrznsC), 
[3](https://scholar.google.com/citations?view_op=view_citation&hl=en&user=IwcnpkwAAAAJ&citation_for_view=IwcnpkwAAAAJ:LkGwnXOMwfcC) 
for more details).

![](http://cKnowledge.org/images/ai-cloud-resize.png)

_Note that at the moment we are very limited with resources and mainly focus on Caffe crowd-benchmarking and crowd-tuning._

Prerequisites
=============
* Collective Knowledge framework ([@GitHub](http://github.com/ctuning/ck))

Installation
============
Obtain CK repository for Tiny DNN:

```
 $ ck pull repo:ck-tiny-dnn
```

Compile simple bench (on Linux/MacOS/Windows; Android G++ has some issues):

```
 $ ck compile program:tiny-dnn-bench --speed
```

Note, that it will automatically install TinyDNN package via CK. 
You can check that it was installed properly via
```
 $ ck show env --tags=tiny-dnn
```

Run this bench
```
 $ ck run program:tiny-dnn-bench
```

Future work
===========
Add Tiny DNN to CK benchmarking and auto-tuning workflow
similar to http://github.com/dividiti/ck-caffe

This is an on-going and long-term project which requires open discussion.
