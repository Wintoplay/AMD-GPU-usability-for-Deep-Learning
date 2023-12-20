# The usability of AMD GPU (7900xtx)
This is just my personal experience and opinions.<br>
I bought RX 7900xtx in November 2023 for Pytorch, Stable diffusion and stuff for 40k THB (~ 1142 USD)

At the present(Dec 2023)

It works work for normal usage of Pytorch, Stable diffusion with ROCM 5.7

I installed Rocm and Pytorch via instruction in https://rocm.docs.amd.com/projects/radeon/en/latest/docs/install/install-radeon.html and https://rocm.docs.amd.com/projects/radeon/en/latest/docs/install/install-pytorch.html

## Benefit of AMD GPU that led the me buying it
* It is far cheaper than Nvidia couterpart.
* Rocm is open-source.

## Limitation and drawback
* Bitsandbytes cannot be used for ROCM 5.7 (Third-party repositories only made it support 5.6)
* Llama CPP only support ROCM 5.6.1 as the latest version of ROCM. When I try to use it. The utilization of shader clock stuck at 100%
* Rocm is not as widely adopted as CUDA yet.