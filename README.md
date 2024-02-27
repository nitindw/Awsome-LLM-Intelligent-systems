# <p align=center>`Awsome-LLM-Modal for Autonomus Driving`<br>
This repo contains a curated list of resources on LLM for Intelligent systems( Autonomous driving, Robotics ..etc) , arranged chronologically. We regularly update it with the latest papers and their corresponding open-source implementations.</p>

<p align="center">
<img src="/Learning3_Methods.gif" width="500" height="500"/>
</p>

<hr />

<img src="\timeline.png" alt="Time Line" />



Authors:[Nitin Dwivedi](https://github.com/nitindw), [Pranav Singh Chib](https://github.com/Pranav-chib) , [Pravendra Singh](https://scholar.google.com/citations?user=YwDTxJMAAAAJ&hl=en) </p>
## Table of Contents

- [Perception](#LEARNING-APPROACHES)
- [Planning](#EXPLAINABILITY)
- [Control](#EVALUATION)
- [Prompt Engineering](#Preparation)
- [Fine Tuning](#Adjustment)
- [Simulation Frameworks](#SAFETY)
- [Datasets](#Large-Language-Models-in-autonomous-driving)
- [CITATION](#Citation)

# Perception
The following are the different Perception approaches of LLM 

## Perception

- [**Driving with LLMs: Fusing Object-Level Vector Modality for Explainable Autonomous Driving**](https://browse.arxiv.org/abs/2310.01957) [arXiv 2023] <br> Long Chen, Oleg Sinavski, Jan Hünermann, Alice Karnsund, Andrew James Willmott, Danny Birch, Daniel Maund, Jamie Shotton <br> [![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/wayveai/Driving-with-LLMs)
  - Backbone: LLaMA
  - Modality: Vector, Language
  - Output: Answer, Actions
<p align="justify">
  Large Language Models (LLMs) have shown promise in the autonomous driving
sector, particularly in generalization and interpretability. This paper introduces a unique
object-level multimodal LLM architecture that merges vectorized numeric modalities with a pre-trained LLM to improve context understanding in driving situations.
We also present a new dataset of 160k QA pairs derived from 10k driving scenarios,
paired with high-quality control commands collected with RL agent and question-answer pairs generated by teacher LLM (GPT-3.5). A distinct pretraining strategy
is devised to align numeric vector modalities with static LLM representations
using vector captioning language data. This paper also introduces an evaluation metric for
Driving QA and demonstrating our LLM driver’s proficiency in interpreting driving
scenarios, answering questions, and decision-making. Our findings highlight the
potential of LLM-based driving action generation compared to traditional
behavioral cloning. We make our benchmark, datasets, and model available 1
for
further exploration.
</p>

- [**Talk2BEV: Language-Enhanced Bird's Eye View Maps**](https://arxiv.org/abs/2310.02251) [arXiv 2023] <br> Vikrant Dewangan, Tushar Choudhary, Shivam Chandhok, Shubham Priyadarshan, Anushka Jain, Arun K. Singh, Siddharth Srivastava, Krishna Murthy Jatavallabhula, K. Madhava Krishna <br> [![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/llmbev/talk2bev)
  - Backbone: Flan5XXL, Vicuna-13b
  - Modality: Vision Language
  - Output: Answer
<p align="justify">
This work introduces Talk2BEV, a large vision language model (LVLM)1
interface for bird’s-eye view (BEV)
maps in autonomous driving contexts. While existing perception
systems for autonomous driving scenarios have largely focused
on a pre-defined (closed) set of object categories and driving
scenarios, Talk2BEV blends recent advances in general-purpose
language and vision models with BEV-structured map representations, eliminating the need for task-specific models. This enables a single system to cater to a variety of autonomous driving
tasks encompassing visual and spatial reasoning, predicting the
intents of traffic actors, and decision-making based on visual
cues. This paper extensively evaluates Talk2BEV on a large number
of scene understanding tasks that rely on both the ability to
interpret free-form natural language queries and in grounding
these queries to the visual context embedded into the language enhanced BEV map. To enable further research in LVLMs
for autonomous driving scenarios, This paper develops and release
Talk2BEV-Bench, a benchmark encompassing 1000 human annotated BEV scenarios, with more than 20,000 questions
and ground-truth responses from the NuScenes dataset.
</p>

## Planning

- [**Talk2BEV: Language-Enhanced Bird's Eye View Maps**](https://arxiv.org/abs/2310.02251) [arXiv 2023] <br> Vikrant Dewangan, Tushar Choudhary, Shivam Chandhok, Shubham Priyadarshan, Anushka Jain, Arun K. Singh, Siddharth Srivastava, Krishna Murthy Jatavallabhula, K. Madhava Krishna <br> [![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/llmbev/talk2bev)
  - Backbone: Flan5XXL, Vicuna-13b
  - Modality: Vision Language
  - Output: Answer
<p align = "justify">
 For safe navigation without human intervention, autonomous driving (AD) systems need to understand the
visual world around them to make informed decisions. This
 entails not just recognizing specific object categories, but also
contextualizing their current and potential future interactions
with the environment. Existing AD systems rely on domain specific models for each scene understanding task, such as
detecting traffic actors and signage or forecasting plausible
future events. On the other hand, recent advances in large
language models (LLMs) and large vision-language
models (LVLMs) have demonstrated a
promising alternative to thinking about perception for AD;
that of a single model pre-trained on web-scale data, capable
of performing all the aforementioned tasks and more (particularly, the ability to deal with unforeseen scenarios). In
this work they ask, how do we most efficiently integrate such
capabilities of LLMs with scene representations traditionally
used in autonomous driving?
</p>

- [**GAIA-1: A Generative World Model for Autonomous Driving**](https://arxiv.org/abs/2309.17080) [arXiv 2023] <br> AnthonyHu, LloydRussell, HudsonYeo, ZakMurez, GeorgeFedoseev,AlexKendall,JamieShotton,andGianlucaCorrado. <br> [![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/taesiri/ArXivQA/blob/main/papers/2309.17080.md)
  - Backbone: GAIA generative model
  - Modality: Vision Language
  - Output: Video
<p align="justify">
Autonomous driving promises transformative improvements to transportation, but
building systems capable of safely navigating the unstructured complexity of
real-world scenarios remains challenging. A critical problem lies in effectively
predicting the various potential outcomes that may emerge in response to the
vehicle’s actions as the world evolves.
To address this challenge, They introduce GAIA-1 (‘Generative AI for Autonomy’),
a generative world model that leverages video, text, and action inputs to generate
realistic driving scenarios while offering fine-grained control over ego-vehicle
behavior and scene features. Our approach casts world modeling as an unsupervised sequence modeling problem by mapping the inputs to discrete tokens, and
predicting the next token in the sequence. Emerging properties from our model
include learning high-level structures and scene dynamics, contextual awareness,
generalization, and understanding of geometry. The power of GAIA-1’s learned
representation that captures expectations of future events, combined with its ability
to generate realistic samples, provides new possibilities for innovation in the field
of autonomy, enabling enhanced and accelerated training of autonomous driving
technology
  </p>
  
 - [**Language Models as Zero-Shot Planners: Extracting Actionable Knowledge for Embodied Agents**](https://arxiv.org/abs/2201.07207) [arXiv 2022] <br> Wenlong Huang, Pieter Abbeel, Deepak Pathak, and Igor Mordatch. <br> [![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/huangwl18/language-planner)
  - Backbone: GPT-3 Codex
  - Modality: Language
  - Output: proposal
- [**Dilu: Aknowledge-driven approach to autonomous driving with large language models**](https://arxiv.org/abs/2309.16292) [arXiv 2023] <br> LichengWen, Daocheng Fu, XinLi, XinyuCai, Tao Ma, PinlongCai, MinDou, BotianShi, LiangHe, and YuQiao. <br> [![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/PJLab-ADG/DiLu)
  - Backbone: GPT-3.5
  - Modality: Language
  - Output: Action
- [**Drive as you speak: Enabling human-like interaction with large language models in autonomous vehicles**](https://openaccess.thecvf.com/content/WACV2024W/LLVM-AD/html/Cui_Drive_As_You_Speak_Enabling_Human-Like_Interaction_With_Large_Language_WACVW_2024_paper.html) [WACV Workshops 2024] <br> CanCui, YunshengMa, XuCao, WenqianYe, andZiran Wang. <br> [![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/PJLab-ADG/DiLu)
  - Backbone: GPT-4
  - Modality: Language
  - Output: code
- [**Receive, Reason,andReact: Drive as You Say with Large Language Models in Autonomous Vehicles**](https://arxiv.org/abs/2310.08034) [arXiv 2023] <br> CanCui, YunshengMa, XuCao, WenqianYe, andZiran Wang. <br> [![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/PJLab-ADG/DiLu)
  - Backbone: GPT-4
  - Modality: Language
  - Output: Answer
- [**Drive Like a Human: Rethinking Autonomous Driving with Large Language Models**](https://arxiv.org/abs/2307.07162) [arXiv 2023] <br> DaochengFu, Xin Li, Licheng Wen, Min Dou, Pinlong Cai, Botian Shi, and Yu Qiao. <br> [![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/PJLab-ADG/DriveLikeAHuman)
  - Backbone: GPT-3.5
  - Modality: Language
  - Output: Answer
- [**Learning to Drive with GPT**](https://arxiv.org/abs/2310.01415) [arXiv 2023] <br> JiagengMao, Yuxi Qian, HangZhao, andYueWang. <br> [![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/PointsCoder/GPT-Driver)
  - Backbone: GPT-3.5
  - Modality: Vision Language
  - Output: Route
- [**SurrealDriver: Designing Generative Driver Agent Simulation Framework in Urban Contexts based on Large Language Model**](https://arxiv.org/abs/2309.13193) [arXiv 2023] <br> Ye Jin, Xiaoxi Shen, HuilingPeng, XiaoanLiu, Jingli Qin, JiayangLi, JintaoXie,PeizhongGao,GuyueZhou, and Jiangtao Gong. <br>
  - Backbone: GPT-4
  - Modality: Language
  - Output: Text, Answer
  
## Control

- [**Driving with LLMs: Fusing Object-Level Vector Modality for Explainable Autonomous Driving**](https://browse.arxiv.org/abs/2310.01957) [arXiv 2023] <br> Long Chen, Oleg Sinavski, Jan Hünermann, Alice Karnsund, Andrew James Willmott, Danny Birch, Daniel Maund, Jamie Shotton <br> [![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/wayveai/Driving-with-LLMs)
  - Backbone: LLaMA
  - Modality: Vector, Language
  - Output: Answer, Actions
- [**Dilu: Aknowledge-driven approach to autonomous driving with large language models**](https://arxiv.org/abs/2309.16292) [arXiv 2023] <br> LichengWen, Daocheng Fu, XinLi, XinyuCai, Tao Ma, PinlongCai,MinDou, BotianShi, LiangHe, and YuQiao. <br> [![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/PJLab-ADG/DiLu)
  - Backbone: GPT-4.0
  - Modality: Language
  - Output: Action
- [**Receive,Reason,andReact:Drive as You Say with Large Language Models in Autonomous Vehicles**](https://arxiv.org/abs/2310.08034) [arXiv 2023] <br> CanCui,YunshengMa,XuCao,WenqianYe, andZiran Wang. <br> [![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/PJLab-ADG/DiLu)
  - Backbone: GPT-4
  - Modality: Language
  - Output: Answer
- [**Drive Like a Human:Rethinking Autonomous Driving with Large Language Models**](https://arxiv.org/abs/2307.07162) [arXiv 2023] <br> DaochengFu,XinLi,LichengWen,MinDou,PinlongCai, BotianShi,andYuQiao. <br> [![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/PJLab-ADG/DriveLikeAHuman)
  - Backbone: GPT-3.5
  - Modality: Language
  - Output: Answer
- [**SurrealDriver: Designing Generative Driver Agent Simulation Framework in Urban Contexts based on Large Language Model**](https://arxiv.org/abs/2309.13193) [arXiv 2023] <br> Ye Jin, Xiaoxi Shen, HuilingPeng, XiaoanLiu, Jingli Qin, JiayangLi, JintaoXie,PeizhongGao,GuyueZhou, and Jiangtao Gong. <br>
  - Backbone: GPT-4
  - Modality: Language
  - Output: Text, Answer
