# UniCoder: Scaling Code Large Language Model via Universal Code

**WIP**

[![](https://img.shields.io/badge/arXiv-2406.16441-b31b1b.svg?style=for-the-badge)](https://arxiv.org/abs/2406.16441)


**Datasets** is open source at [UniCoder-Instruct](https://huggingface.co/datasets/ASC8384/UniCoder-Instruct).

Intermediate reasoning or acting steps have successfully improved large language models (LLMs) for handling various downstream natural language processing (NLP) tasks. When applying LLMs for code generation, recent works mainly focus on directing the models to articulate intermediate natural-language reasoning steps, as in chain-of-thought (CoT) prompting, and then output code with the natural language or other structured intermediate steps. However, such output is not suitable for code translation or generation tasks since the standard CoT has different logical structures and forms of expression with the code. In this work, we introduce the universal code (UniCode) as the intermediate representation. It is a description of algorithm steps using a mix of conventions of programming languages, such as assignment operator, conditional operator, and loop. Hence, we collect an instruction dataset UniCoder-Instruct to train our model UniCoder on multi-task learning objectives. UniCoder-Instruct comprises natural-language questions, code solutions, and the corresponding universal code. The alignment between the intermediate universal code representation and the final code solution significantly improves the quality of the generated code. The experimental results demonstrate that UniCoder with the universal code significantly outperforms the previous prompting methods by a large margin, showcasing the effectiveness of the structural clues in pseudo-code. 

![图片](https://github.com/user-attachments/assets/1852f14b-2177-4a63-8b14-a97d2655c26a)
An example of UniCoder. The Code LLM solves the code generation question by “translating” the pseudocode description (Universal Code) into executable code of the target programming language.

![图片](https://github.com/user-attachments/assets/3620c902-1803-4fe2-932b-17d051cae496)

![图片](https://github.com/user-attachments/assets/5805cb9b-793e-44f5-81f6-5cfda606b348)

![图片](https://github.com/user-attachments/assets/166fefe3-8303-4e37-b2e0-ef83e7c62d08)


## Citation

```bibtex
@article{sun2024unicoder,
  title={Unicoder: Scaling code large language model via universal code},
  author={Sun, Tao and Chai, Linzheng and Yang, Jian and Yin, Yuwei and Guo, Hongcheng and Liu, Jiaheng and Wang, Bing and Yang, Liqun and Li, Zhoujun},
  journal={arXiv preprint arXiv:2406.16441},
  year={2024}
}
```
