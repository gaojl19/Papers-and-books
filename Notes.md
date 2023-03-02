## 2022.3.1
- Directed Diffusion: 
    - DD injects attention into the cross-attention maps for directed prompt words to direct the position of the corresponding objects in the early denoising steps [T, T-N]
    - Strengthen the attention maps of the corresponding additional tokens, and weaken the attention maps of the trailing tokens. 
- Dreambooth
    - learn a unique identifier token that can represent the specific input object through reconstruction loss
    - preserve the model's generalization ability through class preservation loss


## 2022.2.22
- Today I Cliport: This paper proposed a language-conditioned imitation-learning agent that combines the broad semantic understanding (what) of CLIP with the spatial precision (where) of Transporter.
    - Solves language-specified tabletop tasks from packingunseen objects to folding cloths


## 2022.2.20
- Today I read a paper Learning universal policies via text-to-video generation by bkl, this paper proposed to use text-to-video generation to solve sequential manipulation tasks, as these large models pretrained on data available on the Internet can provide better generalization properties.
    - The first problem is combinatorial generalization
        - Env: Painting Factory, same as the PDSketch paper by Mao at MIT
    - The second problem is multi-task generalization
        - Env: a suite of language guided manipulation tasks, same as CLIPort
    - The third problem is real-robot manipulation
        - Env: Bridge dataset