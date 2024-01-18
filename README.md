# <p align=center>`Awsome-LLM-Intelligent-systems`<br>
This repo contains a curated list of resources on LLM for Intelligent systems( Autonomous driving, Robotics ..etc) , arranged chronologically. We regularly update it with the latest papers and their corresponding open-source implementations.</p>

<p align="center">
<img src="/Learning3_Methods.gif" width="500" height="500"/>
<p>

<hr />

# <p align=center>Recent Advancements in End-to-End Autonomous Driving using Deep Learning: A Survey <a href="https://medium.com/@pranavs_chib/end-to-end-autonomous-driving-using-deep-learning-8a94ecb3bb6b">
  <a href="https://medium.com/@pranavs_chib/end-to-end-autonomous-driving-using-deep-learning-8a94ecb3bb6b"> <img align="left" alt="JJ's Medium" src="https://img.shields.io/badge/Medium-12100E?style=for-the-badge&logo=medium&logoColor=white" />
</a>
<a href="https://ieeexplore.ieee.org/document/10258330">
  <img align="left" alt="JJ's Medium" src="https://camo.githubusercontent.com/9505a1887908dd93299cbeedd06bb8bf706b2e5fc69e682bee1375b235ba4009/68747470733a2f2f696d672e736869656c64732e696f2f7374617469632f76313f7374796c653d666f722d7468652d6261646765266d6573736167653d4945454526636f6c6f723d303036323942266c6f676f3d49454545266c6f676f436f6c6f723d464646464646266c6162656c3d" />
</a>
<a href="http://arxiv.org/abs/2307.04370">
  <img align="left" alt="JJ's Medium" src="https://img.shields.io/badge/arXiv-2307.04370-b31b1b.svg" />
</a>
Authors:[Nitin Dwivedi](https://github.com/nitindw), [Pranav Singh Chib](https://github.com/Pranav-chib) </p>
## Table of Contents

- [Perception](#LEARNING-APPROACHES)
- [Planning](#EXPLAINABILITY)
- [Control](#EVALUATION)
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
- [**Talk2BEV: Language-Enhanced Bird's Eye View Maps**](https://arxiv.org/abs/2310.02251) [arXiv 2023] <br> Vikrant Dewangan, Tushar Choudhary, Shivam Chandhok, Shubham Priyadarshan, Anushka Jain, Arun K. Singh, Siddharth Srivastava, Krishna Murthy Jatavallabhula, K. Madhava Krishna <br> [![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/llmbev/talk2bev)
  - Backbone: Flan5XXL, Vicuna-13b
  - Modality: Vision Language
  - Output: Answer


## Planning
- [**Talk2BEV: Language-Enhanced Bird's Eye View Maps**](https://arxiv.org/abs/2310.02251) [arXiv 2023] <br> Vikrant Dewangan, Tushar Choudhary, Shivam Chandhok, Shubham Priyadarshan, Anushka Jain, Arun K. Singh, Siddharth Srivastava, Krishna Murthy Jatavallabhula, K. Madhava Krishna <br> [![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/llmbev/talk2bev)
  - Backbone: Flan5XXL, Vicuna-13b
  - Modality: Vision Language
  - Output: Answer
- [**GAIA-1: A Generative World Model for Autonomous Driving**](https://arxiv.org/abs/2309.17080) [arXiv 2023] <br> AnthonyHu, LloydRussell, HudsonYeo, ZakMurez, GeorgeFedoseev,AlexKendall,JamieShotton,andGianlucaCorrado. <br> [![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/taesiri/ArXivQA/blob/main/papers/2309.17080.md)
  - Backbone: GAIA generative model
  - Modality: Vision Language
  - Output: Video
 - [**Language Models as Zero-Shot Planners: Extracting Actionable Knowledge for Embodied Agents**](https://arxiv.org/abs/2201.07207) [arXiv 2022] <br> WenlongHuang,PieterAbbeel,DeepakPathak, andIgor Mordatch. <br> [![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/huangwl18/language-planner)
  - Backbone: GPT-3 Codex
  - Modality: Language
  - Output: proposal
- [**Dilu: Aknowledge-driven approach to autonomous drivingwith large languagemodels**](https://arxiv.org/abs/2309.16292) [arXiv 2023] <br> LichengWen, Daocheng Fu, XinLi, XinyuCai, Tao Ma, PinlongCai,MinDou, BotianShi, LiangHe, and YuQiao. <br> [![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/PJLab-ADG/DiLu)
  - Backbone: GPT-3.5
  - Modality: Language
  - Output: Action
- [**Drive as you speak: Enabling human-like interaction with large language models in autonomous vehicles**](https://openaccess.thecvf.com/content/WACV2024W/LLVM-AD/html/Cui_Drive_As_You_Speak_Enabling_Human-Like_Interaction_With_Large_Language_WACVW_2024_paper.html) [WACV Workshops 2024] <br> CanCui,YunshengMa,XuCao,WenqianYe, andZiran Wang. <br> [![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/PJLab-ADG/DiLu)
  - Backbone: GPT-4
  - Modality: Language
  - Output: code
- [**Receive,Reason,andReact:Drive as You Say with Large Language Models in Autonomous Vehicles**](https://arxiv.org/abs/2310.08034) [arXiv 2023] <br> CanCui,YunshengMa,XuCao,WenqianYe, andZiran Wang. <br> [![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/PJLab-ADG/DiLu)
  - Backbone: GPT-4
  - Modality: Language
  - Output: Answer
- [**Drive Like a Human:Rethinking Autonomous Driving with Large Language Models**](https://arxiv.org/abs/2307.07162) [arXiv 2023] <br> DaochengFu,XinLi,LichengWen,MinDou,PinlongCai, BotianShi,andYuQiao. <br> [![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/PJLab-ADG/DriveLikeAHuman)
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
