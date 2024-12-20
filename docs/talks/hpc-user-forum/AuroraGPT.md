# AuroraGPT
Ray Yang
2024-09-04

## 🎯 AuroraGPT Goals

<div class="flex-container"
style="flex-direction: column; justify-content: space-around;">

<div class="flex-container"
style="flex-direction: row; justify-content: space-around; align-items:center;">

<div class="col1">

<div class="blue-card" style="margin-bottom: 0.5em;">

**AuroraGPT**: *General purpose scientific LLM*  
Broadly trained on a general corpora plus scientific {papers, texts,
data}

</div>

- **Explore pathways** towards a “Scientific Assistant” model
- **Build with international partners** (RIKEN, BSC, others)
- **Multilingual** English, 日本語, French, German, Spanish
- **Multimodal**: images, tables, equations, proofs, time series,
  graphs, fields, sequences , etc

</div>

<div class="col2" style="width:75%; text-align: center;">

![](https://github.com/Hannibal046/Awesome-LLM/raw/main/resources/image8.gif)

<span class="dim-text" style="font-size: 75%;">Image from
[`Hannibal046/Awesome-LLM`](https://github.com/Hannibal046/Awesome-LLM)</span>

</div>

</div>

<div id="fig-timeline">

<img src="./assets/timelines.png"
style="margin-left:auto;margin-right:auto;;width:66.0%" />


Figure 1: Credit to the entire AuroraGPT team for slides.

</div>

</div>

<div class="notes">

- Here to talk about AuroraGPT, Argonne’s internal effort to build a
  general purpose scientific LLM, broadly trained on a general corpora
  of text + scientific {papers, text, data}

- As part of this effort, we plan to…

  - Explore pathways, build with international partners, multi-{lingual,
    modal}

- Rough timeline of the project and deliverables:

  - 202{3,4}: text-only models, plan to release a series of {7B, 70B,
    1T} models
  - 202{4,5}: Basic multi-modal models
  - 202{5,6}: Advanced scientific multimodal models

</div>

## 🧪 AuroraGPT: Open Science Foundation Models

<div style="vertical-align:center;">

![](./assets/AuroraGPT.svg)

</div>

<div class="notes">

- AuroraGPT will be a publicly distributed, open source foundation model
  for open science
- Is being trained on:
  - Scientific / engineering structured data
  - General text, media, news, etc.
  - Large amounts of low to medium quality data
  - Much less high quality data (that is publicly available for use)
- This data is then cleaned, processed, de-duplicated and used for the
  initial pre-training phase of the model
- The vast majority of the overall compute is spent during this initial
  pre-training phase
  - This is the group I help to lead and will be talking a bit about
    today
- The initial pre-training phase is currently underway
  - Eventually, given a bit of time, effort and magic, the model will be
    ready for fine-tuning and additional training for a variety of
    downstream tasks
- The pretrained model will then be handed off for additional
  fine-tuning on a variety of downstream tasks
  - Scientific discovery
  - Accelerate scientific tasks
  - Digital twins
  - Inverse design
  - Code optimization
  - Accelerated simulations
  - Autonomous experiments
  - Co-design
- Becoming increasingly clear that LLMs have the potential to
  drastically accelerate computational science
  - We’ve seen this already for {GenSLMs, Weather / Climate / Earth
    Systems Modeling, Particle Physics, etc.}

</div>

## 📊 AuroraGPT Outcomes

- **Datasets and data pipelines** for preparing science training data
- **Software infrastructure and workflows** to train, evaluate and
  deploy LLMs at scale for scientific resarch purposes
- **Evaluation of state-of-the-art LLM Models** to determine where they
  fall short in deep scientific tasks and where deep data may have an
  impact
- **Assessment of the approach** of augmenting web training data with
  two forms of data specific to science
  - Full text scientific papers
  - Structured scientific datasets (suitably mapped to narrative form)
- **Research grade artifacts** (**models**) for scientific community for
  adaptation for downstream uses
- **Promotion of responsible AI** best practices where we can figure
  them out
- **International Collaborations** around the long term goal of *AGI for
  science*

<div class="notes">

- Deliverables:

  - datasets, pipelines
  - software infrastructure, workflows to interface with science
    applications
  - checkpoints, models, logs, workbook, insights, etc.

- Hope to understand:

  - How different state-of-the-art models perform at different
    scientific tasks
  - where deep data may have an impact
  - feasibility of generically augmenting text with scientific
    structured data

- Huge undertaking that will require large international collaborations
  around long term goal of AGI for science

- Extra points:

  - Well known that LLMs are good for non-consequential tasks
  - Known to “hallucinate” and create false information
  - Can this be mitigated reliably ??

</div>

## 🌌 Aurora

<div class="flex-container">

<div class="col1">

<div id="tbl-aurora">

Table 1: Aurora Specs

| <!-- --> | <!-- --> |
|----------|:--------:|
| Racks    |   166    |
| Nodes    |  10,624  |
| CPUs     |  21,248  |
| GPUs     |  63,744  |
| NICs     |  84,992  |
| HBM      |   8 PB   |
| DDR5c    |  10 PB   |
| <!-- --> | <!-- --> |

</div>

</div>

<div id="fig-aurora">

![](./assets/aurora.png)


Figure 2: [Aurora Fact
Sheet](https://www.alcf.anl.gov/sites/default/files/2024-07/Aurora_FactSheet_2024.pdf)

</div>

</div>

## 🤖 ALCF AI Testbed

- ALCF AI Testbed Systems are in production and [available for
  allocations](https://accounts.alcf.anl.gov/#/allocationRequests) to
  the research community
- Significant improvement in time-to-solution and energy-efficiency for
  diverse AI for science applications.
- [NAIRR Pilot](https://nairrpilot.org/)

<div class="red-card" style="color: #FF5252; font-size:90%;">

Up to 25X improvement for genomic foundation models with 6.5X energy
efficiency

</div>

<div class="flex-container" style="margin-bottom: 1em;">

<div id="fig-sambanova">

![](./assets/sambanova.jpeg)


Figure 3: **SambaNova SN-30**: 2nd Gen, 8 nodes with 64 AI Accelerators

</div>
<div id="fig-graphcore">

![](./assets/graphcore.png)


Figure 4: **Graphcore Bow**: generation accelerators: Pod-64
configuration with 64 accelerators

</div>
<div id="fig-cerebras">

![](./assets/cerebras.jpeg)


Figure 5: **Cerebras**: 2x CS-2 WSE with Memory-X and Swarm-X
technologies

</div>
<div id="fig-groq">

![](./assets/groq.jpeg)


Figure 6: **GroqRack**: 9 nodes, 8 GroqChip v1.5 Tensor streaming
processors accelerators per node

</div>

</div>

## 👥 Team Leads

<!--
&#10;| Team                  | Lead(s)           |                                                            |
| :----:                | :--------         | :--------------------------------------------------------: |
| **Planning**          | Rick Stevens      | ![](./assets/team/rick-stevens.png){height="40pt"}         |
|                       | Ian Foster        | ![](./assets/team/ian-foster.png){height="40pt"}           |
|                       | Rinku Gupta       | ![](./assets/team/rinku-gupta.png){height="40pt"}          |
|                       | Mike Papka        | ![](./assets/team/mike-papka.png){height="40pt"}           |
|                       | Fangfang Xia      | ![](./assets/team/fangfang-xia.png){height="40pt"}         |
| **Data**              | Ian Foster        | ![](./assets/team/ian-foster.png){height="40pt"}           |
|                       | Robert Underwood  | ![](./assets/team/robert-underwood.png){height="40pt"} |
| **Models + Training** | Venkat Vishwanath | ![](./assets/team/venkat.jpg){height="40pt"}               |
|                       | Sam Foreman       | ![](./assets/team/sam-foreman.png){height="40pt"}          |
|                       | Sam Foreman       | ![](./assets/team/sam-foreman.png){height="40pt"}          |
| **Inference**         | Eliu Huerta       | ![](./assets/team/eliu-huerta.png){height="40pt"}          |
|                       | Azton Wells       | ![](./assets/team/azton-wells.png){height="40pt"}          |
: Team Leads {#tbl-team-leads}
| **Models / Training** | Venkat Vishwanath | ![](./assets/team/venkat-vishwanath.png){height="40pt"} |
|                       | Robert Underwood  | ![](./assets/team/robert-underwood.png){height="40pt"}     |
-->

<div style="font-size: 66%;">

<div class="flex-container"
style="text-align: center; align-items: center;">

**Planning**

<img src="./assets/team/rick-stevens.png" style="height:1.04167in"
alt="Rick Stevens" />

<img src="./assets/team/ian-foster.png" style="height:1.04167in"
alt="Ian Foster" />

<img src="./assets/team/rinku-gupta.png" style="height:1.04167in"
alt="Rinku Gupta" />

<img src="./assets/team/mike-papka.png" style="height:1.04167in"
alt="Mike Papka" />

<img src="./assets/team/arvind-ramanathan.png" style="height:1.04167in"
alt="Arvind Ramanathan" />

<img src="./assets/team/fangfang-xia.png" style="height:1.04167in"
alt="Fangfang Xia" />

</div>

<div class="flex-container" style="text-align: center;">

<div class="col2">

**Data**

<img src="./assets/team/ian-foster.png" style="height:1.04167in"
alt="Ian Foster" />

<img src="./assets/team/robert-underwood.png" style="height:1.04167in"
alt="Robert Underwood" />

</div>

<div class="col2">

**Models / Training**

<img src="./assets/team/venkat-vishwanath.png" style="height:1.04167in"
alt="Venkat Vishwanath" />

<img src="./assets/team/sam-foreman.png" style="height:1.04167in"
alt="Sam Foreman" />

</div>

<div class="col2">

**Evaluation**

<img src="./assets/team/franck-cappello.png" style="height:1.05556in"
alt="Franck Cappello" />

<img src="./assets/team/sandeep-madireddy.png" style="height:1.04167in"
alt="Sandeep Madireddy" />

<img src="./assets/team/bo-li.png" style="height:1.04167in"
alt="Bo Li" />

</div>

<div class="col2">

**Post**

<img src="./assets/team/eliu-huerta.png" style="height:1.04167in"
alt="Eliu Huerta" />

<img src="./assets/team/azton-wells.png" style="height:1.04167in"
alt="Azton Wells" />

</div>

<div class="col2">

**Inference**

<img src="./assets/team/rajeev-thakur.png" style="height:1.04167in"
alt="Rajeev Thakur" />

</div>

<div class="col2">

**Comms**

<img src="./assets/team/charlie-catlett.png" style="height:1.04167in"
alt="Charlie Catlett" />

<img src="./assets/team/david-martin.png" style="height:1.04167in"
alt="David Martin" />

</div>

<div class="col2">

**Distribution**

<img src="./assets/team/brad-ullrich.png" style="height:1.04167in"
alt="Brad Ullrich" />

</div>

</div>

</div>

## 🤝 Teams

<div class="flex-container">

<div class="col1">

- **Planning**
- **Data Prep**
  - Accumulate 20+ T tokens of high-quality scientific text and
    structured data
- <span style="background: oklch(from #ff1a8f calc(l * 1.15) c h / 0.1); border: 1px solid #ff1a8f; border-radius: 0.25px;">**Models
  / Training**</span>[^1]
  - Train (entirely from scratch) a series of models on publicly
    available data
- **Evaluation**
  - Skills, trustworthiness, safety, robustness, privacy, machine ethics

</div>

<div class="col2">

- **Post-Training**
  - Fine-tuning, alignment
- **Inference**
  - Model serving, API development / public-facing web services
- **Distribution**
  - Licensing, generating and distributing artifacts for public
    consumption
- **Communication**

</div>

</div>

## 🦜 Model Training

<div class="flex-container"
style="text-align: left; width: 100%; justify-content: space-around; line-height: 1em;">

<div class="col1" width="48%"
style="background: oklch(from #03BD00 calc(l * 1.15) c h / 0.1); border: 1px solid #03BD00; border-radius: 0.25em; padding: 3pt 8pt; margin-left: 5pt; margin-right: 5pt;">

✅ <span style="color: #03BD00;">**Goals**</span>

- Want training runs at scale to be:
  - efficient
  - stable
  - reproducible
- This requires:
  - robust data pipelines / file IO
  - effectively overlapping compute with communication
  - stability across {network, filesystem, machine}
- 3D / Multi-dimensional Parallelism strategies
- Large batch training
- Second order optimizers
- Sub-quadratic attention
- State space models
- *Highly optimized GPU kernels*

</div>

<div class="col2" width="48%"
style="background: oklch(from #E90102 calc(l * 1.15) c h / 0.1); border: 1px solid #E90102; border-radius: 0.25em; padding: 3pt 8pt; margin-left: 5pt; margin-right: 5pt;">

❌ <span style="color: #E90102;">**Challenges**</span>

- *Looong time* to train, can be:
  - weeks (even months) of continuous training
  - order of magnitude longer than typical NN training jobs
- Stability issues:
  - failures are expensive (but inevitable)
  - stragglers common at scale
- Individual jobs are:
  - **fragile**
  - only as good as the worst rank
  - one hang or bad worker can crash job
  - network / filesystem / other-user(s) dependent
- Cost / benefits of different collective communication algorithms
  - depend on optimized / efficient implementations
- Network performance
- *Highly optimized GPU kernels*

</div>

</div>

<div class="aside">

[`argonne-lcf/Megatron-DeepSpeed`](https://github.com/argonne-lcf/Megatron-DeepSpeed)

</div>

## 🚀 Accelerating Dataset Processing at Scale for Training

- To train a fixed model on trillions of tokens requires:
  - Aggregating data from multiple different *corpora* (e.g. Reddit,
    StackExchange, GitHub, etc.)
  - Sampling *each training batch* according to a fixed distribution
    across corpora
  - Building indices that map batches of tokens into these files
    (indexing)
- The original implementation was slow, and designed to run on a single
  device
  - Major bottleneck when debugging data pipeline at scale
- [x] Completely re-wrote an asynchronous, distributed implementation
  that *significantly* improves performance

## 🚀 Accelerating Dataset Processing at Scale for Training

- [x] Completely re-wrote an asynchronous, distributed implementation
  that *significantly* improves performance

<div class="columns">

<div class="column">

![Time spent building `BlendableDataset`](./assets/blendable.svg)

</div>

<div class="column">

![Time spent building `GPTDataset`](./assets/gpt.svg)

</div>

</div>

## 📓 References

<div class="flex-container" style="gap: 1em;">

<div class="col1">

- 🏡 [samforeman.me](https://samforeman.me):
  - 🦜 [Talks](https://samforeman.me/talks/):
    - [HPC User Forum](https://samforeman.me/talks/hpc-user-forum/)
      \[[slides](https://samforeman.me/talks/hpc-user-forum/slides.html)\]
- See my other slides on:
  - [LLMs from Scratch](https://saforem2.github.io/llm-workshop-talk)
  - [Creating Small(~ish) LLMs](https://saforem2.github.io/LLM-tutorial)
  - [Parallel Training
    Techniques](https://saforem2.github.io/parallel-training-slides)
  - [LLMs on
    Polaris](https://samforeman.me/talks/llms-on-polaris/#/title-slide)
  - [Training LLMs at Scale](https://samforeman.me/talks/llms-at-scale/)

</div>

<div class="col2">

- [🏎️
  `argonne-lcf/Megatron-DeepSpeed`](https://github.com/argonne-lcf/Megatron-DeepSpeed)  
  <span class="dim-text">For the largest of large language
  models.</span>
- [🍋 `saforem2/ezpz`](https://github.com/saforem2/ezpz)  
  <span class="dim-text">Distributed training, ezpz.</span>
- 👀 See also:
  - [New international consortium for generative AI models for
    science](https://www.anl.gov/article/new-international-consortium-formed-to-create-trustworthy-and-reliable-generative-ai-models-for)
  - [PyTorch Distributed
    Overview](https://pytorch.org/tutorials/beginner/dist_overview.html)
  - [Distributed Data Parallel — PyTorch master
    documentation](https://pytorch.org/docs/master/notes/ddp.html)
  - [🤗 Efficient Training on Multiple
    GPUs](https://huggingface.co/docs/transformers/en/perf_train_gpu_many)
  - [Getting Started -
    DeepSpeed](https://www.deepspeed.ai/getting-started/)

</div>

</div>

### ❤️ Thank you!

- Organizers

- Feel free to reach out!

  <split even>

  [<i class="fas fa-home"></i>](https://samforeman.me)
  [<i class="far fa-paper-plane"></i>](mailto:///foremans@anl.gov)
  [<i class="fab fa-twitter"></i>](https://www.twitter.com/saforem2)

  </split>

> [!NOTE]
>
> ### 🙏 Acknowledgements
>
> This research used resources of the Argonne Leadership Computing
> Facility, which is a DOE Office of Science User Facility supported
> under Contract DE-AC02-06CH11357.

### 📑 Bibliography

- Refs:
  - (**wei2022emergentabilitieslargelanguage?**)
  - Animations from [The Illustrated
    Transformer](http://jalammar.github.io/illustrated-transformer/)

<div id="refs">

</div>

## 🎁 Extras

### 🚂 Loooooooooong Sequence Lengths

<!-- ::: {.flex-container style="text-align: center; align-items: center;"} -->
<!-- ![](../../assets/anl.svg){style="width:48%;"} -->

<div class="flex-container"
style="align-items: center; justify-content: center;">

<img src="../../assets/anl.svg" style="height:50pt;" />

<span class="dim-text" style="font-size: 2.0em;"></span>

<img src="../../assets/deepspeed-logo-transparent.svg"
style="height:50pt;" />

</div>

<!--
[]{.dim-text style="font-size: 2.0em; padding-left: 15pt;"}
![](../../assets/deepspeed-logo-transparent.svg){style="width: 60%"}
:::
-->

- Working with [
  Microsoft/DeepSpeed](https://github.com/microsoft/DeepSpeed) team to
  enable longer sequence lengths (context windows) for LLMs
  - See my [blog
    post](https://samforeman.me/posts/auroragpt/long-sequences/) for
    additional details

<div id="fig-long-seq">

<div class="flex-container">

![25B](https://raw.githubusercontent.com/saforem2/scaling4science/main/assets/25B.svg)

![33B](https://raw.githubusercontent.com/saforem2/scaling4science/main/assets/33B.svg)

</div>

Figure 7: Maximum (achievable) `SEQ_LEN` for both `25B` and `33B` models
(See: (**song2023ds4sci?**))

</div>

<div class="aside">

[ `scaling4science`](https://github.com/saforem2/scaling4science)  
[
`Megatron-DS-Benchmarking`](https://github.com/saforem2/Megatron-DS-Benchmarking)

</div>

### ♻️ Life Cycle of the LLM

<div class="panel-tabset" style="text-align:center">

#### 📝 Pre-training

<div id="fig-pretraining">

![](https://jalammar.github.io/images/gpt3/03-gpt3-training-step-back-prop.gif)


Figure 8: **Pre-training**: Virtually all of the compute used during
pretraining phase

</div>

#### 🎀 Fine-Tuning

<div id="fig-fine-tuning">

![](https://jalammar.github.io/images/gpt3/10-gpt3-fine-tuning.gif)


Figure 9: **Fine-tuning**: Fine-tuning actually updates the model’s
weights to make the model better at a certain task.

</div>

</div>

### 🍎 Training LLMs

<div class="flex-container" style="align-items: flex-end;">

<div class="col1" style="width:33%;">

<div id="fig-it-hungers">

![](https://github.com/saforem2/llm-lunch-talk/blob/main/docs/assets/it_hungers.jpeg?raw=true)


Figure 10: It’s hungry!

</div>

</div>

<div class="col2" style="width:60%;">

<div id="fig-evolution">

![](https://github.com/Mooler0410/LLMsPracticalGuide/raw/main/imgs/survey-gif-test.gif)


Figure 11: Visualization from (**yang2023harnessing?**)

</div>

</div>

</div>

<!--
### 💾 Evaluating Checkpoints {background-color="white"}
&#10;```python
from typing import Optional
import os
from pathlib import Path
&#10;from transformers import LlamaForCausalLM, AutoTokenizer
&#10;tokenizer = AutoTokenizer.from_pretrained("meta-llama/Llama-2-7B-hf")
&#10;def load_model(ckpt_dir) -> LlamaForCausalLM:
    return LlamaForCausalLM.from_pretrained(ckpt_dir)
&#10;def eval_model(model, max_length: int, prompt: str) -> str:
    return (
        tokenizer.batch_decode(
            model.generate(
                **tokenizer(prompt, return_tensors="pt"),
                 max_length=max_length,
            ),
            clean_up_tokenization_spaces=True,
            skip_special_tokens=True,
        )[0]
    )
&#10;def load_and_eval_model_from_checkpoint(
        step: int,
        max_length: int = 64,
        prompt: Optional[str] = None,
        ckpt_root: Optional[os.PathLike | Path | str] = None,
) -> str:
    print(f"Loading model from checkpoint at global step: {step}")
    prompt = "What is it like in there?" if prompt is None else prompt
    ckpt_root = Path("checkpoints") if ckpt_root is None else Path(ckpt_root)
    ckpt_dir = ckpt_root.joinpath(f"global_step{step}")
    return (
        eval_model(
            model=load_model(ckpt_dir.as_posix())
            max_length=max_length,
            prompt=prompt,
        )
    )
```
&#10;### Model Evaluations {background-color="white"}
&#10;::: {.panel-tabset}
&#10;#### 7000
&#10;Tokens: 88B
&#10;```python
>>> print(load_checkpoint(7000))
Loading model from checkpoint at global step: 7000
"What is it like in there?"
"""
I'm not sure if it's a good idea to use a different name for the same thing,
but I'm sure it's a good idea to use a different name for the same thing.
I'm not sure if it's a good idea to use a different name for the same thing,
but I'm sure it's a good idea to use a different name for the same thing.
I'm not sure if it's a good idea to use a different name for the same thing,
but I'm sure it
"""
```
&#10;#### 12000
&#10;Tokens: 150B
&#10;```python
>>> print(load_checkpoint(12000))
Loading model from checkpoint at global step: 12000
"What is it like in there?"
"""
What is it like in there?
The people are very friendly and helpful.
What is it like in there?
The people are very friendly and helpful.
What is it like in there?
The people are very friendly and helpful.
What is it like in there?
The people are very friendly and helpful.
What is it like in there?
The people are very friendly and helpful.
What is it like in there?
"""
```
&#10;#### 17000
&#10;Tokens: 215B
&#10;```python
>>> print(load_checkpoint(17000))
Loading model from checkpoint at global step: 17000
"What is it like in there?"
"""
I’m not sure what to expect. I’m not sure what to expect from the people I’m
with. I’m not sure what to expect from the people I’m with. I’m not sure what
to expect from the people I’m with. I’m not sure what to expect from the people
I’m with.
I’m not sure what to expect from the people I’m with.
I’m not sure what to expect from the people I’m with.
I’m not sure what to expect from the people
"""
```
&#10;#### 22000
&#10;Tokens: 277B
&#10;```python
>>> print(load_checkpoint(22000))
Loading model from checkpoint at global step: 22000
"What is it like in there?"
"""
I’m a 20 year old guy from the UK. I’m a student at the University of
Manchester, studying Computer Science. I’m a big fan of the band, The Beatles,
and I’m a huge fan of the movie, The Wizard of Oz. I’m a huge fan of the band,
The Beatles, and I’m a huge fan of the movie, The Wizard of Oz.
I’m a big fan of the band, The Beatles, and I’m a huge fan of the movie
"""
```
&#10;#### 32000
&#10;Tokens: 400B
&#10;```python
>>> print(load_checkpoint(32000))
Loading model from checkpoint at global step: 32000
"What is it like in there?"
"""
I've been to the US and I've been to Canada.
In the US, it's a lot like the US.
In Canada, it's a lot like the US.
In the US, it's a lot like the US.
In Canada, it's a lot like the US.
In the US, it's a lot like the US.
In Canada, it's a lot like the US.
In the US, it's
"""
```
&#10;#### 40000
&#10;Tokens: 503B
&#10;```python
>>> print(load_checkpoint(40000))
Loading model from checkpoint at global step: 40000
"What is it like in there?"
"""
The first thing you notice when you enter the room is the size. It’s huge. It’s
like a football field. It’s a lot of space.
The second thing you notice is the light. It’s bright. It’s bright.
The third thing you notice is the sound. It’s loud. It’s loud.
The fourth thing you notice is the smell. It’s a lot of smells. It’s a lot of smells.
The fifth thing you notice is the temperature. It’s hot.
"""
```
&#10;:::
-->
<!-- ::: -->
<!--
- Being trained on:
&#10;  :::: {.flex-container style="flex-direction:row; justify-content: space-around;"}
&#10;  ::: {.flex-container style="flex-direction:column;"}
&#10;   🇺🇸English  
   🇯🇵日本語  
   🇫🇷French  
   🇩🇪Deutsch  
   🇪🇸Español[^bsc]  
   🇮🇹Italian  
&#10;  :::
&#10;  ::: {.flex-container style="flex-direction:column;"}
&#10;  🧪 scientific text  
  🖼️ images  
  📊 tables  
  ➕ equations  
  📖 proofs
&#10;  :::
&#10;  ::: {.flex-container style="flex-direction:column;"}
&#10;  📆 structured data  
  ⛓️ sequences  
  ⏰ time-series  
  🕸️ graphs  
  🌀 fields
&#10;  :::
&#10;  ::::
&#10;[^riken]:|
    [Argonne and RIKEN sign a MOU in support of AI for science](https://www.anl.gov/article/argonne-and-riken-sign-a-memorandum-of-understanding-in-support-of-ai-for-science)
&#10;[^bsc]:|
    Collaborations with Barcelona Supercomputing Center
&#10;-->

[^1]: Co-led by: Venkat Vishwanath, Sam Foreman
