# IQMA
PyTorch code for NTIRE challenge IQA method "IQMA Network: Image Quality Multi-scale Assessment Network"

# Questions?
I reproduce the code for the NTIRE challenge IQA method "IQMA Network: Image Quality Multi-scale Assessment Network", but I got some problems:
1. In the original paper, the size of four stages feature maps extracted from the pretrained ResNet-50 is C ∗ 8 ∗ 8, C ∗ 4 ∗ 4, C ∗ 2 ∗ 2 and C ∗ 1 ∗ 1, respectively. Then, these features are concatenated to group (Fjrefi, Fjdisti, Fjrefi− Fjdisti), respectively. Finally, the concatenated features are go through two convolutional layers with size 3x3 and 2x2 for further feature extraction. Here is the question, for the 3C ∗ 4 ∗ 4, 3C ∗ 2 ∗ 2 and 3C ∗ 1 ∗ 1 features maps, how can the two convolutional layers can effectively extract the features? Espectially for the 3C ∗ 1 ∗ 1 features maps? 
2. According to my implement, the SRCC and PLCC results are hard to reach 0.700 on the validation set, what's the reason? Are there any fatal errors in my code?
