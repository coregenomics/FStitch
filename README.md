#FStitch
##Usage
Scientists looking to classify regions of high read density in Globab Run On sequencing will find Fast Read Stitcher (FStitch) most useful as it identifies putative nascent transcripts __de novo__. However, users may also find this package useful as a ChIP-seq peak caller.
##System Requirements
FStitch is written in the C++ programming language and uses OpenMP to parallelize portions of the program.  With this in mind, users will need to have a GCC compilers later than version 4.2 to compile and run FStitch. For mac users, downloading the latest Xcode will update the GCC compiler need be. To check you compiler version, 

$gcc —-version

or 

$g++ —-version

Note, for those running FStitch on a compute cluster, commonly you will need to perform a ‘module load gcc<version>’ to compile FStitch. Please ask your sys admins for questions on module load behavior. 
##Setup
If your compiler is up to date, you can compile FStitch by moving into the FastReadStitcher/ directory and running 

$sh setup.sh

This runs “make” in the src/ directory. If everything compiles, you should see at the end of the compilation:

$=========================================

$Sucessfully Compiled

Importantly, will you now see the executable “FStitch” in the src directory. This will be the command used for the following computations. 

##train
FStitch uses two probabilistic models to classify regions of high read density that may be indicative of nascent transcription (GRO-seq) or read coverage peak (ChIP-seq): Logistic Regression and a Hidden Markov Model. Commonly 
\begin{equation}
4*5
\end{equation}





###parameters
##segment
###parameters
## Understanding and Interpreting Output


