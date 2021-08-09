# Quality Assessment of In-the-Wild Videos
[![License](https://img.shields.io/github/license/mashape/apistatus.svg?maxAge=2592000)](License)

## Description
VSFA code for the following papers:

- Dingquan Li, Tingting Jiang, and Ming Jiang. [Quality Assessment of In-the-Wild Videos](https://dl.acm.org/citation.cfm?doid=3343031.3351028). In Proceedings of the 27th ACM International Conference on Multimedia (MM ’19), October 21-25, 2019, Nice, France. [[arxiv version]](https://arxiv.org/abs/1908.00375)

## Get Started

1. Install requirements
2. Run `python test.py -i video.mp4 -n 50`

Currently the process is inefficiet, because

  - We restrict the torch device to be CPU.
  - We load all frames into memory by skvideo, which may cause OOM.
    - Therefore we can only test on about **50 frames**.
  - We use huge patch.

