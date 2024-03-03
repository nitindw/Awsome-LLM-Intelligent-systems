# <p align=center>`Awsome-LLM-Modal for Autonomous Driving`<br>
This repo contains a curated list of resources on LLM for Intelligent systems( Autonomous driving, Robotics ..etc), arranged chronologically. We regularly update it with the latest papers and their corresponding open-source implementations.</p>

<p align="center">
<img src="/Learning3_Methods.gif" width="500" height="500"/>
</p>

<hr />

<img src="\timeline.png" alt="Time Line" />



Authors:[Nitin Dwivedi](https://github.com/nitindw), [Pranav Singh Chib](https://github.com/Pranav-chib) , [Pravendra Singh](https://scholar.google.com/citations?user=YwDTxJMAAAAJ&hl=en) </p>
## Table of Contents

- [Perception](#Perception)
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
They also present a new dataset of 160k QA pairs derived from 10k driving scenarios,
paired with high-quality control commands collected with RL agent and question-answer pairs generated by teacher LLM (GPT-3.5). A distinct pretraining strategy
is devised to align numeric vector modalities with static LLM representations
using vector captioning language data. This paper also introduces an evaluation metric for
Driving QA and demonstrating our LLM driver’s proficiency in interpreting driving
scenarios, answering questions, and decision-making. Our findings highlight the
potential of LLM-based driving action generation compared to traditional
behavioral cloning. They make our benchmark, datasets, and model available 1
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
interpret free-form natural language queries and grounding
these queries to the visual context embedded into the language-enhanced BEV map. To enable further research in LVLMs
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
with the environment. Existing AD systems rely on domain-specific models for each scene understanding task, such as
detecting traffic actors and signage or forecasting plausible
future events. On the other hand, recent advances in large
language models (LLMs) and large vision-language
models (LVLMs) have demonstrated a
a promising alternative to thinking about perception for AD;
that of a single model pre-trained on web-scale data, capable
of performing all the aforementioned tasks and more (particularly, the ability to deal with unforeseen scenarios). In
this work they ask, how do They most efficiently integrate such
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
real-world scenarios remain challenging. A critical problem lies in effectively
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
<p align = "justify">
  Can world knowledge learned by large language models (LLMs) be used to act in
interactive environments? In this paper, They investigate the possibility of grounding
high-level tasks, expressed in natural language (e.g. “make breakfast”), to a chosen
set of actionable steps (e.g. “open fridge”). While prior work focused on learning
from explicit step-by-step examples of how to act, They surprisingly find that if
pre-trained LMs are large enough and prompted appropriately, they can effectively
decompose high-level tasks into mid-level plans without any further training. However, the plans produced naively by LLMs often cannot map precisely to admissible
actions. They propose a procedure that conditions on existing demonstrations and
semantically translates the plans to admissible actions. Our evaluation in the recent
VirtualHome environment shows that the resulting method substantially improves
executability over the LLM baseline. The conducted human evaluation reveals a
trade-off between executability and correctness but shows a promising sign towards
extracting actionable knowledge from language models
</p>

- [**Dilu: Aknowledge-driven approach to autonomous driving with large language models**](https://arxiv.org/abs/2309.16292) [arXiv 2023] <br> LichengWen, Daocheng Fu, XinLi, XinyuCai, Tao Ma, PinlongCai, MinDou, BotianShi, LiangHe, and YuQiao. <br> [![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/PJLab-ADG/DiLu)
  - Backbone: GPT-3.5
  - Modality: Language
  - Output: Action
<p align = "justify">
  Recent advancements in autonomous driving have relied on data-driven approaches, which are widely adopted but face challenges including dataset bias,
overfitting, and uninterpretability. Drawing inspiration from the knowledge-driven
nature of human driving, They explore the question of how to instill similar capabilities into autonomous driving systems and summarize a paradigm that integrates an interactive environment, a driver agent, as well as a memory component
to address this question. Leveraging large language models (LLMs) with emergent abilities, They propose the DiLu framework, which combines Reasoning and
a Reflection module to enable the system to perform decision-making based on
common-sense knowledge and evolve continuously. Extensive experiments prove
DiLu’s capability to accumulate experience and demonstrate a significant advantage in generalization ability over reinforcement learning-based methods. Moreover, DiLu is able to directly acquire experiences from real-world datasets which
highlights its potential to be deployed on practical autonomous driving systems.
To the best of our knowledge, They are the first to leverage knowledge-driven capability in decision-making for autonomous vehicles. Through the proposed DiLu
framework, LLM is strengthened to apply knowledge and to reason causally in the
autonomous driving domain.
</p>

- [**Drive as you speak: Enabling human-like interaction with large language models in autonomous vehicles**](https://openaccess.thecvf.com/content/WACV2024W/LLVM-AD/html/Cui_Drive_As_You_Speak_Enabling_Human-Like_Interaction_With_Large_Language_WACVW_2024_paper.html) [WACV Workshops 2024] <br> CanCui, YunshengMa, XuCao, WenqianYe, andZiran Wang. <br> [![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/PJLab-ADG/DiLu)
  - Backbone: GPT-4
  - Modality: Language
  - Output: code
<p align="justify">
  The future of autonomous vehicles lies in the convergence of human-centric design and advanced AI capabilities. Autonomous vehicles of the future will not only transport passengers but also interact and adapt to their desires, making the journey comfortable, efficient, and pleasant. In this paper, They present a novel framework that leverages Large Language Models (LLMs) to enhance autonomous vehicles' decision-making processes. By integrating LLMs' natural language capabilities and contextual understanding, specialized tools usage, synergizing reasoning, and acting with various modules on autonomous vehicles, this framework aims to seamlessly integrate the advanced language and reasoning capabilities of LLMs into autonomous vehicles. The proposed framework holds the potential to revolutionize the way autonomous vehicles operate, offering personalized assistance, continuous learning, and transparent decision-making, ultimately contributing to safer and more efficient autonomous driving technologies.
</p>

- [**Receive, Reason,andReact: Drive as You Say with Large Language Models in Autonomous Vehicles**](https://arxiv.org/abs/2310.08034) [arXiv 2023] <br> CanCui, YunshengMa, XuCao, WenqianYe, andZiran Wang. <br> [![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/PJLab-ADG/DiLu)
  - Backbone: GPT-4
  - Modality: Language
  - Output: Answer
<p align="justify">
The fusion of human-centric design and artificial
intelligence (AI) capabilities has opened up new possibilities for
next-generation autonomous vehicles that go beyond transportation. These vehicles can dynamically interact with passengers
and adapt to their preferences. This paper proposes a novel
framework that leverages Large Language Models (LLMs) to
enhance the decision-making process in autonomous vehicles. By
utilizing LLMs’ linguistic and contextual understanding abilities
with specialized tools, they aim to integrate the language and
reasoning capabilities of LLMs into autonomous vehicles. Our
research includes experiments in HighwayEnv, a collection of
environments for autonomous driving and tactical decision-making tasks, to explore LLMs’ interpretation, interaction,
and reasoning in various scenarios. They also examine real-time personalization, demonstrating how LLMs can influence
driving behaviors based on verbal commands. Their empirical
results highlight the substantial advantages of utilizing chain-of-thought prompting, leading to improved driving decisions,
and showing the potential for LLMs to enhance personalized driving experiences through ongoing verbal feedback. The
proposed framework aims to transform autonomous vehicle
operations, offering personalized support, transparent decision-making, and continuous learning to enhance safety and effectiveness. They achieve user-centric, transparent, and adaptive
autonomous driving ecosystems supported by the integration of
LLMs into autonomous vehicles.
</p>

- [**Drive Like a Human: Rethinking Autonomous Driving with Large Language Models**](https://arxiv.org/abs/2307.07162) [arXiv 2023] <br> DaochengFu, Xin Li, Licheng Wen, Min Dou, Pinlong Cai, Botian Shi, and Yu Qiao. <br> [![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/PJLab-ADG/DriveLikeAHuman)
  - Backbone: GPT-3.5
  - Modality: Language
  - Output: Answer
<p align="justify">
In this paper, They explore the potential of using a large language model (LLM) to understand the driving environment in a human-like manner and analyze its ability to reason, interpret, and memorize when facing complex scenarios. They argue that traditional optimization-based and modular autonomous driving (AD) systems face inherent performance limitations when dealing with long-tail corner cases. To address this problem, they propose that an ideal AD system should drive like a human, accumulating experience through continuous driving and using common sense to solve problems. To achieve this goal, They identify three key abilities necessary for an AD system: reasoning, interpretation, and memorization. They demonstrate the feasibility of employing an LLM in driving scenarios by building a closed-loop system to showcase its comprehension and environment-interaction abilities. Our extensive experiments show that the LLM exhibits the impressive ability to reason and solve long-tailed cases, providing valuable insights for the development of human-like autonomous driving.
</p>

- [**Learning to Drive with GPT**](https://arxiv.org/abs/2310.01415) [arXiv 2023] <br> JiagengMao, Yuxi Qian, HangZhao, andYueWang. <br> [![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/PointsCoder/GPT-Driver)
  - Backbone: GPT-3.5
  - Modality: Vision Language
  - Output: Route
<p align="justify">
They present a simple yet effective approach that can transform the OpenAI GPT-3.5 model into a reliable motion planner for autonomous vehicles. Motion planning is a core challenge in autonomous driving, aiming to plan a driving trajectory that is safe and comfortable. Existing motion planners predominantly leverage heuristic methods to forecast driving trajectories, yet these approaches demonstrate insufficient generalization capabilities in the face of novel and unseen driving scenarios. In this paper, they propose a novel approach to motion planning that capitalizes on the strong reasoning capabilities and generalization potential inherent to Large Language Models (LLMs). The fundamental insight of our approach is the reformulation of motion planning as a language modeling problem, a perspective not previously explored. Specifically, They represent the planner inputs and outputs as language tokens and leverage the LLM to generate driving trajectories through a language description of coordinate positions. Furthermore, they propose a novel prompting-reasoning-finetuning strategy to stimulate the numerical reasoning potential of the LLM. With this strategy, the LLM can describe highly precise trajectory coordinates and also its internal decision-making process in natural language. They evaluate our approach on the large-scale nuScenes dataset, and extensive experiments substantiate the effectiveness, generalization ability, and interpretability of our GPT-based motion planner.
</p>

- [**SurrealDriver: Designing Generative Driver Agent Simulation Framework in Urban Contexts based on Large Language Model**](https://arxiv.org/abs/2309.13193) [arXiv 2023] <br> Ye Jin, Xiaoxi Shen, HuilingPeng, XiaoanLiu, Jingli Qin, JiayangLi, JintaoXie, PeizhongGao, GuyueZhou, and Jiangtao Gong. <br>
  - Backbone: GPT-4
  - Modality: Language
  - Output: Text, Answer
<p align="justify">
Simulation plays a critical role in the research and development of autonomous driving and intelligent transportation systems. However, the current simulation platforms exhibit limitations in the realism and diversity of agent behaviors, which impede the transfer of simulation outcomes to the real world. In this paper, they propose a generative driver agent simulation framework based on large language models (LLMs), capable of perceiving complex traffic scenarios and providing realistic driving maneuvers. Notably, they conducted interviews with 24 drivers and used their detailed descriptions of driving behavior as chain-of-thought prompts to develop a `coach agent' module, which can evaluate and assist driver agents in accumulating driving experience and developing human-like driving styles. Through practical simulation experiments and user experiments, they validate the feasibility of this framework in generating reliable driver agents and analyze the roles of each module. The results show that the framework with full architect decreased the collision rate by 81.04% and increased the human-likeness by 50%. Our research proposes the first urban context driver agent simulation framework based on LLMs and provides valuable insights into the future of agent simulation for complex tasks.
</p>

## Control

- [**Driving with LLMs: Fusing Object-Level Vector Modality for Explainable Autonomous Driving**](https://browse.arxiv.org/abs/2310.01957) [arXiv 2023] <br> Long Chen, Oleg Sinavski, Jan Hünermann, Alice Karnsund, Andrew James Willmott, Danny Birch, Daniel Maund, Jamie Shotton <br> [![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/wayveai/Driving-with-LLMs)
  - Backbone: LLaMA
  - Modality: Vector, Language
  - Output: Answer, Actions
<p align="justify">
With camera sensors being one of the most common sensors used in autonomous driving <a href="https://www.mdpi.com/1424-8220/23/6/3335">Sensor fusion in autonomous vehicle
with traffic surveillance camera system: Detection, localization, and ai networking</a>, a
natural step to incorporate language has been through VLMs. For example <a href="https://proceedings.mlr.press/v100/roh20a.html">Conditional driving from natural
language instructions </a>uses images and
language directions to train a driving policy. <a href="https://openaccess.thecvf.com/content_CVPR_2020/html/Kim_Advisable_Learning_for_Self-Driving_Vehicles_by_Internalizing_Observation-to-Action_Rules_CVPR_2020_paper.html">Advisable learning for self-driving vehicles by internalizing observation-to-action rules</a> proposes a method for learning vehicle control with
human assistance. The system learns to summarize its visual observations in natural language, predict
an appropriate action response (e.g. “I see a pedestrian crossing, so I stop”), and predict the controls,
accordingly. Using language to explain the inner workings of the model has also been explored in
<a href="https://arxiv.org/abs/2302.00673">Adapt Action-aware driving caption transformer</a>, where user-friendly natural language narrations and reasoning are provided for each decision
making step of autonomous vehicular control and action.
In robotics, They have seen efforts to fuse language with other modalities. Albeit outside of the autonomous
driving field, the closest work to ours [38] utilizes point clouds with 3D bounding boxes of potential
object candidates. It also uses a language utterance referring to a target object in the scene to train a
model capable of identifying a target object from a set of potential candidates. Recently, the RT-2
paper [39] demonstrated a similar approach by utilizing LLMs for low-level robotics control tasks,
including the joint training of VQA and control tasks. However, their framework is confined to the
vision modality, whereas They introduce a novel methodology for grounding vector-based object level
modalities into LLMs, facilitating interpretable control and driving QA tasks. In contrast to these
existing efforts, the work presented in this paper is, to the best of our knowledge, the first to fuse
numeric vector modality with language specifically in the domain of autonomous vehicles.
</p>

- [**Dilu: Aknowledge-driven approach to autonomous driving with large language models**](https://arxiv.org/abs/2309.16292) [arXiv 2023] <br> LichengWen, Daocheng Fu, XinLi, XinyuCai, Tao Ma, PinlongCai, MinDou, BotianShi, LiangHe, and YuQiao. <br> [![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/PJLab-ADG/DiLu)
  - Backbone: GPT-4.0
  - Modality: Language
  - Output: Action
<p align="justify">
Drawing inspiration from the profound question posed by LeCun (2022):<b> “Why can an adolescent learn to drive a car in about 20 hours of practice and know how to act in many situations"</b>
he/she has never encountered before?”, They explore the core principles that underlie human driving
skills and raise a pivotal distinction: human driving is fundamentally knowledge-driven, as opposed
to data-driven. For example, when faced with a situation where the truck ahead is in danger of
losing its cargo, humans can rely on common sense and explainable reasoning to ensure a safe distance is maintained between vehicles. Conversely, data-driven methods rely on a large quantity of similar data to fit this scenario which lacks environment comprehension and limits generalization
ability <a href="https://ieeexplore.ieee.org/abstract/document/9575933">An application-driven conceptualization of corner
cases for perception in highly automated driving</a>, <a href="https://ieeexplore.ieee.org/abstract/document/9963987">Milestones in autonomous driving and intelligent vehicles: Survey of surveys</a>, and <a href="https://arxiv.org/abs/2302.06803">Bringing diversity to autonomous vehicles: An interpretable multi-vehicle decision-making and planning framework</a>. Furthermore, this task requires
significant human labor and financial resources to collect and annotate driving data to handle varied
real-world scenarios. This observation catalyzes a fundamental question:<b> How can They instill such
knowledge-driven capabilities of human drivers into an autonomous driving system?</b>
</p>
<p align="justify">
  In terms of the setup for highway-env, They directly obtain vehicle information from the underlying
simulation and input it into the scenario descriptor. This information only includes each vehicle’s
position, speed, and acceleration data in the current frame, without any decision intent or potential
risk information, as shown in Figure 8. Meta-actions are used as the decision output in our experiments, which include five discrete actions to control the ego vehicle: acceleration, maintaining
speed, deceleration, and lane changes to the left and right. For each closed-loop driving task, They
define a successful completion time of 30 seconds, with a decision-making frequency of 1Hz. This
means that if the ego vehicle can navigate through traffic at a reasonable speed and without collisions for 30 seconds, They consider the task to be successfully completed. Unless otherwise stated,
our experimental environment is a four-lane motorway with a vehicle density of 2.0, representing
scenarios with relatively high traffic density and complexity. All other settings follow the simulator’s
default configurations.

</p>

- [**Receive,Reason,andReact:Drive as You Say with Large Language Models in Autonomous Vehicles**](https://arxiv.org/abs/2310.08034) [arXiv 2023] <br> CanCui,YunshengMa,XuCao,WenqianYe, andZiran Wang. <br> [![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/PJLab-ADG/DiLu)
  - Backbone: GPT-4
  - Modality: Language
  - Output: Answer
<p align="justify">
Imagine a situation where you are in control of an autonomous vehicle, and you feel the front vehicle is too slow
and desire to safely overtake that vehicle. All you have to do
is speak out the command, ”Pass the vehicle in front of me.”
At that point, the LLMs would assess the existing conditions
and safety considerations in real time, providing you with
informed guidance on the feasibility and recommended actions
for executing the maneuver. Furthermore, in the context of
fully autonomous vehicles, the LLMs’ capabilities could even
extend to taking charge of the vehicle and executing the
instructed commands.</p>
<p align="justify">
The promise of integrating LLMs into autonomous driving
systems is enormous. It holds the potential to enhance the
safety, efficiency, and user experience of autonomous vehicles
in novel ways. By gathering the vast knowledge and reasoning
abilities of these models, vehicles are not only self-driving but
also highly adaptive, capable of understanding and responding
to the complex interactions of the road.
</p>
<p align="justify">
To address the challenge above, They present a novel approach
where LLMs serve as the decision-making “brain” within autonomous vehicles. Complementing this, various tools within
the autonomous vehicle ecosystem, including the perception
module, localization module, and in-cabin monitor, function as
the vehicle’s sensory “eyes.” This configuration enables LLMs
to overcome the inherent limitation of not directly accessing
real-time environmental information. Additionally, the vehicle’s controller function as its “hands,” executing instructions
derived from the LLM’s decision-making process. Through
receiving environmental information and drivers’ commands,
reasoning based on this information and human interaction,
and finally making decisions, They make the autonomous driving
experience that is not just technologically superior but also
deeply human-centric by LLMs. This approach gains even
more credibility through experiments conducted in various
driving scenarios, providing proof of LLMs’ revolutionalizing
potential in the realm of autonomous vehicles.
</p> 

- [**Drive Like a Human:Rethinking Autonomous Driving with Large Language Models**](https://arxiv.org/abs/2307.07162) [arXiv 2023] <br> DaochengFu,XinLi,LichengWen,MinDou,PinlongCai, BotianShi,andYuQiao. <br> [![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/PJLab-ADG/DriveLikeAHuman)
  - Backbone: GPT-3.5
  - Modality: Language
  - Output: Answer
<p align="justify">
Towards the goal of driving like a human, They identify three abilities that are necessary: 1) Reasoning:
Given a specific driving scenario, the model should be able to make decisions by reasoning via
common sense and experience. 2) Interpretation The decisions made by the agent should able to be
interpreted. This demonstrates the ability of introspection and the existence of declarative memory.
3) Memorization: After reasoning and interpreting scenarios, a memory mechanism is required to
remember previous experiences and enable the agent to make similar decisions once facing similar
situations.
Based on the above three properties, They refer to the paradigm of human learning to drive and condense
a canonical form of a driving system. This schema includes four modules:
(1) Environment creates a stage that the agent can interact with by the interaction flow; (2) Agent
stands for a driver that can perceive the environment and make decisions utilizing its memory and
learning from expert advice; (3) Memory allows the agent to accumulate experience and perform
actions with it via the reflection flow; and (4) Expert provides advice on agent training and gives
feedback when it acts inconsistently, which forms the supervision flow. To be specific, as a universal
driving framework, the Environment, the Agent, and the Expert can be represented by the real-world
or simulator, human drivers or driving algorithms, and simulator or instructor feedback, respectively.
</p>
<img src="\control.webp" alt="GPT-3.5 closed loop driving" />
<p align="justify">
The main contributions of this paper are as follows:
<ol type="1">
<li>They dive deep into how to make autonomous driving systems drive like a humans to prevent
catastrophic forgetting of the existing AD systems when facing long-tail corner cases and
summarized into three key abilities to drive like a human: Reasoning, Interpretation and
Memorization.</li>
<li>They are the first to demonstrate the feasibility of employing LLM in driving scenarios and
exploit its decision-making ability in the simulated driving environment.</li>
<li>Extensive experiments in our study express impressive comprehension and the ability to
solve long-tailed cases. They hope that these insights will inspire academia and industry to
contribute to the development of human-like autonomous driving.</li></ol>
</p>

- [**SurrealDriver: Designing Generative Driver Agent Simulation Framework in Urban Contexts based on Large Language Model**](https://arxiv.org/abs/2309.13193) [arXiv 2023] <br> Ye Jin, Xiaoxi Shen, HuilingPeng, XiaoanLiu, Jingli Qin, JiayangLi, JintaoXie, PeizhongGao, GuyueZhou, and Jiangtao Gong. <br>
  - Backbone: GPT-4
  - Modality: Language
  - Output: Text, Answer
<p align="justify">
Simulation plays a critical role in the research and development of autonomous driving and intelligent transportation systems. However, the current simulation platforms exhibit limitations in the realism and diversity of agent behaviors, which impede the transfer of simulation outcomes to the real world. In this paper, They propose a generative driver agent simulation framework based on large language models (LLMs), capable of perceiving complex traffic scenarios and providing realistic driving maneuvers. Notably, They conducted interviews with 24 drivers and used their detailed descriptions of driving behavior as chain-of-thought prompts to develop a `coach agent' module, which can evaluate and assist driver agents in accumulating driving experience and developing human-like driving styles. Through practical simulation experiments and user experiments, They validate the feasibility of this framework in generating reliable driver agents and analyze the roles of each module. The results show that the framework with full architect decreased the collision rate by 81.04% and increased the human-likeness by 50%. Our research proposes the first urban context driver agent simulation framework based on LLMs and provides valuable insights into the future of agent simulation for complex tasks.
</p>
