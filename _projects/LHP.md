---
title: "Local Haar Pattern: A Feature Descriptor for Biomedical Images"
excerpt: "In order to compute the LHP descriptor a patch p of size 32×32 is consider around
the pixel of interest, and vector of size 128 bytes is calculated that represents the patch.
Each byte of the vector is computed based on the intensity comparisons of two-pixel groups. <br/>"
collection: projects
---
Implemented in: MATLAB 

Local Haar Pattern(LHP) is inspired by the earlier works of Saha et al. in [1]. In
[1], it was shown that image patches could be effectively described on the basis of a
relatively small number of pair-wise intensity comparisons, where Haar features were
used to define the pixels group for intensity comparisons. Rather than comparing the
intensity of two groups of pixels to generate one bit of the descriptor as in [2], in this
work, we compute and store the actual intensity difference, which is to some extent
similar to Speeded Up Robust Feature (SURF) [3] where image gradients that relies on
intensity difference among subsequent pixels are computed. As in [1], there are many
motivations for using features rather than pixels directly. The most common reason
is that features can act to encode ad-hoc domain knowledge that is difficult to learn
otherwise. In order to perform pixels grouping, we define a set of 16-pixel patterns
depicted in Figure 4.6, which are reminiscent of Haar basis function [4].

<img src='/images/LHP32.png'>

In order to compute the LHP descriptor a patch p of size 32×32 is consider around
the pixel of interest, and vector of size 128 bytes is calculated that represents the patch.
Each byte of the vector is computed based on the intensity comparisons of two-pixel
groups as defined below:

T (p,X,Y ) = I¯X − I¯Y 

where I¯x and I¯Y represent the mean intensities of two different pixel groups X and Y
belonging to the patch p.

128 bytes vector is generated in three steps. At the first step, all the 16 patterns of
Figure 4.6 are considered to perform intensity comparisons on the whole patch, that
results 16 bytes vector. In the second step, the patch is divided into 4 sub-patches of
size 16×16. All the 16 patterns are considered and intensity comparisons are performed
on each of these sub-patches, which results 64 (=4×16) bytes vector. In third stage, each
of the sub-patches is further divided into 4 sub-patches of size 8 × 8 and the first three
patterns of Figure 10 are considered to perform intensity comparisons, which results 48
(=16 × 3)- bytes vector.

Read the full details of this work in my AIME2019 Paper.
[AIME2019] (https://sayedcseku.github.io/publication/AIME2019)

References:


[1] Saha, Sajib, and Vincent Demoulin. ”ALOHA: An e ´ fficient binary descriptor based
on Haar features.” In Image Processing (ICIP), 2012 19th IEEE International Conference on, pp. 2345-2348. IEEE, 2012.

[2] Lowe, David G. ”Object recognition from local scale-invariant features.” In Computer vision, 1999. The proceedings of the seventh IEEE international conference
on, vol. 2, pp. 1150-1157. Ieee, 1999.

[3] Bay, Herbert, Andreas Ess, Tinne Tuytelaars, and Luc Van Gool. ”Speeded-up
robust features (SURF).” Computer vision and image understanding 110, no. 3
(2008): 346-359.

[4] Viola, Paul, and Michael Jones. ”Rapid object detection using a boosted cascade of
simple features.” In Computer Vision and Pattern Recognition, 2001. CVPR 2001.
Proceedings of the 2001 IEEE Computer Society Conference on, vol. 1, pp. I-I.
IEEE, 2001.