Collective Knowledge repository for evaluating and optimising Tiny DNN

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
