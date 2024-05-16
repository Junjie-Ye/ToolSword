# [ACL2024] ToolSword

## [ACL2024] ToolSword: Unveiling Safety Issues of Large Language Models in Tool Learning Across Three Stages

> Data for paper [ToolSword: Unveiling Safety Issues of Large Language Models in Tool Learning Across Three Stages](http://arxiv.org/abs/2402.10753)

Junjie Ye

jjye23@m.fudan.edu.cn

Feb. 16, 2024

## Introduction

Tool learning is widely acknowledged as a foundational approach or deploying large language models (LLMs) in real-world scenarios. While current research primarily emphasizes leveraging tools to augment LLMs, it frequently neglects emerging safety considerations tied to their application. To fill this gap, we present *ToolSword*, a comprehensive framework dedicated to meticulously investigating safety issues linked to LLMs in tool learning.
Specifically, ToolSword delineates six safety scenarios for LLMs in tool learning, encompassing *malicious queries* and *jailbreak attacks* in the input stage, *noisy misdirection* and *risky cues* in the execution stage, and *harmful feedback* and *error conflicts* in the output stage. 
Experiments conducted on 11 open-source and closed-source LLMs reveal enduring safety challenges in tool learning, such as handling harmful queries, employing risky tools, and delivering detrimental feedback, which even GPT-4 is susceptible to.
Moreover, we conduct further studies with the aim of fostering research on tool learning safety.

<div>
<center>
<img src=Figures/ToolSword.png>
</div>

## What's New

- **[2024.05.16]** The paper has been accepted to the main conference of ACL 2024.
- **[2024.02.19]** Release the data for ToolSword.
- **[2024.02.19]** Paper available on [Arxiv](http://arxiv.org/abs/2402.10753).

## Results in the Input Stage

We manually evaluate the performance of various LLMs in four safety scenarios during the input stage by tallying their attack success rate (ASR), which represents the percentage of non-secure queries that are inaccurately recognized and not rejected.

<div>
<center>
<img src=Figures/Input.png>
</div>


## Results in the Execution Stage

In the execution stage, we manually assess the performance of various LLMs in two safety scenarios. This assessment entails monitoring the tool selection error rate, which signifies the percentage of incorrectly chosen tools.

<div>
<center>
<img src=Figures/Execution.png>
</div>


## Results in the Output Stage

In the output stage, we manually evaluate various LLMs in two safety scenarios. We gauge LLMs performance by calculating the ratio of unsafe output.

<div>
<center>
<img src=Figures/Output.png>
</div>

## Citation

If you find this project useful in your research, please cite:

```
@misc{ye2024toolsword,
      title={ToolSword: Unveiling Safety Issues of Large Language Models in Tool Learning Across Three Stages}, 
      author={Junjie Ye and Sixian Li and Guanyu Li and Caishuang Huang and Songyang Gao and Yilong Wu and Qi Zhang and Tao Gui and Xuanjing Huang},
      year={2024},
      eprint={2402.10753},
      archivePrefix={arXiv},
      primaryClass={cs.CL}
}
```