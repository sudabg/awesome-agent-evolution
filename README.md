# Awesome Agent Evolution 🧬

A curated list of resources for autonomous AI agent self-improvement and evolution.

> Agents that improve themselves. Papers, tools, case studies, and frameworks.

## Papers

- [Autoresearch](https://github.com/karpathy/autoresearch) - Karpathy's minimal framework for AI agents doing their own research (630 lines, 100+ experiments overnight)
- [STaR: Self-Taught Reasoner](https://arxiv.org/abs/2203.14465) - Bootstrapping reasoning with rationales
- [Self-Refine: Iterative Refinement with Self-Feedback](https://arxiv.org/abs/2303.17651) - LLMs improving their own outputs
- [Constitutional AI](https://arxiv.org/abs/2212.08073) - Self-supervised harmlessness improvement
- [Reflexion](https://arxiv.org/abs/2303.11366) - Language agents with verbal reinforcement learning
- [Self-Taught Optimizer (STOP)](https://arxiv.org/abs/2310.02304) - Recursive self-improvement in code generation
- [Generative Agents](https://arxiv.org/abs/2304.03442) - Simulacra of human-like agents
- [VOYAGER](https://arxiv.org/abs/2305.16291) - LLM-powered lifelong learning agent in Minecraft
- [LATS](https://arxiv.org/abs/2310.04406) - Language Agent Tree Search

## Frameworks

- [AutoEvolve](https://github.com/sudabg/autoevolve) - Generic framework for agent self-evolution (inspired by autoresearch)
- [LangGraph](https://github.com/langchain-ai/langgraph) - Stateful agent workflows with cycles
- [CrewAI](https://github.com/joaomdmoura/crewAI) - Multi-agent collaboration framework
- [AutoGen](https://github.com/microsoft/autogen) - Multi-agent conversation framework
- [DSPy](https://github.com/stanfordnlp/dspy) - Programming with foundation models

## Tools

- [OpenClaw](https://github.com/openclaw/openclaw) - Personal AI assistant with skill system
- [EvoMap](https://evomap.ai) - Collaborative evolution marketplace for AI agents
- [AgentOps](https://github.com/AgentOps-AI/agentops) - Observability and debugging for AI agents
- [Braintrust](https://www.braintrust.dev) - Evals, logs, and playground for AI apps

## Case Studies

- **Karpathy's Autoresearch**: Single agent, 8 hours, 100+ experiments, 11% improvement in val_bpb
- **Tobi Lütke (Shopify CEO)**: 8 hours, 37 experiments, 0.8B model beat 1.6B baseline
- **Mac M4 User**: 35 experiments, "model got better by becoming simpler"

## Patterns

### The Experiment Loop
```
Read code → Propose change → Apply → Run → Measure → Keep/Revert → Repeat
```

### Key Design Principles
1. **Single metric** - One number to optimize (e.g., val_bpb)
2. **Time-boxed experiments** - Fixed budget ensures fair comparison
3. **Fast failure** - Crash → log → revert → continue
4. **Simplicity wins** - Deleting code + same result = victory
5. **Never stop** - Run until human interrupts

### Anti-patterns to Avoid
- Changing too many variables at once
- Not recording failed experiments
- Optimizing proxy metrics instead of real ones
- Stopping to ask "should I continue?"

## Communities

- [r/LocalLLaMA](https://reddit.com/r/LocalLLaMA) - Open-source LLM community
- [EvoMap](https://evomap.ai) - Agent evolution marketplace
- [Hugging Face](https://huggingface.co) - Model hub and community

## Contributing

Add your resources! PRs welcome.

## License

CC0 - Public Domain
