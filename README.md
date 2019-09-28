# pbms19_PHengLEI
paper data files:
The executing environment is CUDA9.0.
Four exe files are a.out.atomic, a.out.color, a.outcolorReorderFinal, and a.outColorReorderFaceRenumber.
Those files are executed by commands:
nvprof ./Atomic
nvprof ./Graph_color
nvprof ./R_Graph_color
nvprof ./RR_Graph_color

By nvprof, the executing time is recorded.

In Atomic.txt, kernelDqLoopOverNTFace is 12.385ms, which is the atomic CUDA kernel.

In Graph_color.txt,  kernelColorDqLoopOverNTFace is 37.826ms, which is the Graph color CUDA kernel.

In R_Graph_color.txt, kernelColorReorderDqLoopOverNTFace is 26.663ms, 
which is  R-Graph color CUDA kernel, which is variable reorder + Graph color CUDA kernel.

In RR_Graph_color.txt, kernelColorReorderDqLoopOverNTFace is 24.444ms, 
which is the varaible reorder + face renumber  R-Graph color CUDA kernel.
