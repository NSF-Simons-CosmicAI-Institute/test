# AstroVisBench
## Description
AstroVisBench is a benchmark for evaluating Large Language Models on scientific computing and data visualization tasks specific to astronomy, enabling systematic assessment of AI code generation capabilities for astronomical data analysis.

Authors:
Sebastian Joseph

Working Group 1 - Explorable Universe

Link to complete repository: https://github.com/NSF-Simons-CosmicAI-Institute/AstroVisBench

## Research Motivation
This benchmark was developed to address the lack of domain-specific evaluation frameworks for assessing LLM performance on astronomy code tasks. It directly supports CosmicAI's Explorable Universe goal of building trustworthy AI assistants (AstroCopilot) by providing standardized metrics to measure progress in multi-modal LLM capabilities for astronomical research, including data processing, analysis pipelines, and scientific visualization generation.


## Usage
Users first set up the conda environment using the provided requirements, download the benchmark environment and optional ground truth cache. The benchmark JSON file contains astronomy queries with setup, processing, and visualization tasks that must be filled by an LLM. Execution is performed via exec_bench.py which runs the generated code against ground truth, evaluating processing correctness through variable inspection and visualization quality through LLM-as-judge evaluation. Results are aggregated using aggregate_results.py to produce success rates and error distributions.


## License
CC BY-SA 4.0


## Citation
```
@misc{joseph2025astrovisbenchcodebenchmarkscientific,
      title={AstroVisBench: A Code Benchmark for Scientific Computing and Visualization in Astronomy}, 
      author={Sebastian Antony Joseph and Syed Murtaza Husain and Stella S. R. Offner and Stéphanie Juneau and Paul Torrey and Adam S. Bolton and Juan P. Farias and Niall Gaffney and Greg Durrett and Junyi Jessy Li},
      year={2025},
      eprint={2505.20538},
      archivePrefix={arXiv},
      primaryClass={cs.CL},
      url={https://arxiv.org/abs/2505.20538}
}
```
