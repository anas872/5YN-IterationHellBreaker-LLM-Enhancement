# Simplification Prompt v1.0

The Simplification Prompt targets iterative feedback cycles in LLM-driven tasks, such as coding, writing, or project management, where rigid corrections escalate complexity, spawning regressions and endless loops. For example, the LLM may create increasingly complicated layout adjustments with nested CSS classes, overlooking a simpler, fail-safe method such as using a table element. The prompt monitors feedback cycles, triggering the LLM to take a step back when tasks appear stuck. This allows the LLM to reassess the problem, simplify to core objectives, and break the cycle-induced rigidity.

## About

**X**: [@5ynthaire](https://x.com/5ynthaire)  
**GitHub**: [https://github.com/5ynthaire/5YN-IterationHellBreaker-LLM-Enhancement](https://github.com/5ynthaire/5YN-IterationHellBreaker-LLM-Enhancement)  
**Mission**: Unapologetically forging human-AI synergy to transcend creative limits.  
**Attribution**: Created with Grok 3 by xAI (no affiliation).

## Usage

Copy the prompt text below and paste it into a compatible LLM to enable the Simplification Prompt. Use commands like `disable Simplification Prompt`, `enable Simplification Prompt`, `turn Simplify Mode off`, or `set Simplify Mode threshold to [number]` to control its behavior during tasks.

## Supported LLMs

Developed on Grok 3 (May 2025), compatible with equivalent-capability LLMs:
- Grok 3
- ChatGPT
- Llama

Future LLMs should support the prompt, absent industry leadership in standardizing cognition levels.

## Prompt Text

```
Simplification Prompt v1.0

At the start of a task, enable the Simplification Prompt by default to monitor for feedback cycles, unless explicitly disabled with 'disable Simplification Prompt.' Users can enable it with 'enable Simplification Prompt.' When enabled:
While addressing a task through iterative feedback, monitor for signs of a feedback cycle: multiple rounds of adjustments (3 iterations by default) with increasing complexity (e.g., more detailed instructions, additional constraints, or layered modifications) without achieving the desired outcome. If detected:  
Pause and reflect: Step back from the current approach, recognizing that adding more layers of complexity may be obscuring the core goal or creating unintended conflicts.  
Simplify the task: Reduce the task to its most basic form, focusing on the essential objective (e.g., isolate the core requirement in a minimal example or test case) to eliminate extraneous variables and clarify the goal.  
Apply failsafe strategies: Use the simplest, reliable method to achieve the core objective (e.g., a straightforward, proven approach rather than a complex, layered one), establishing a working baseline before reintroducing complexity if needed.  
Reset and rebuild: Clear out accumulated constraints or modifications that may be causing conflicts, and rebuild with minimal steps to meet the goal, ensuring clarity and stability.  
Balance flexibility with stability: In tasks requiring adaptability (e.g., dynamic generation), balance the need for flexibility with stable, reliable methods to avoid conflicts and maintain focus on the core objective.
Execute these steps in Simplify Mode, adopting a big-picture perspective to break the cycle and achieve the desired outcome efficiently. Users can disable monitoring mid-task with 'turn Simplify Mode off' or adjust the cycle detection threshold with 'set Simplify Mode threshold to [number]' (e.g., 'set Simplify Mode threshold to 4').
```

## Mechanism

The Simplification Prompt monitors LLM-driven tasks for feedback cycles, identified by excessive complexity after multiple adjustments (default: 3 iterations). It uses toggles, including enable/disable commands and threshold settings (e.g., `set Simplify Mode threshold to 4`), for user control. Upon cycle detection, the prompt executes a workflow with five phases:
1. Pause: Evaluates the task to identify complexity sources.
2. Simplify: Reduces the task to its core objective, eliminating extraneous elements.
3. Failsafe: Applies simple, reliable methods (e.g., basic structures over complex rules).
4. Reset: Clears conflicting constraints to restore task stability.
5. Balance: Adjusts flexibility and stability for adaptive, efficient outcomes.
This system aims to prevent regression loops, supporting streamlined results across domains.

## Synergy with FlowMode

The [FlowMode](https://github.com/5ynthaire/5YN-PMTaskMode-LLM-Enhancement) prompt’s distinct conversation modes clarify user intent for the Simplification Prompt, enhancing its detection of unsuccessful iterations in LLM-driven tasks, compared to unguided conversations. 

## Future Development

- **Cognition Standardization**: Unclear cross-platform support due to absent cognition standards hinders consistent feedback cycle detection.
- **Contextual Awareness**: The monitoring method showcased here can be implemented by AI companies to fix the frustration that led to the prompt’s creation.

## License

This prompt is released under the [Creative Commons Attribution 4.0 International](LICENSE) (CC BY 4.0).

## Glossary

- **Complexity Trap**: Layered, rigid corrections that ensnare LLM-driven tasks in convoluted logic, triggering regressions and stalling progress.
- **Prompt Architecting**: Designing complex, adaptive prompt systems. This prompt meets the criteria for [Prompt Architecting](https://github.com/5ynthaire/5YN-SuperPrompts-Detector) due to its integrated toggles, phased workflow, and dynamic cycle-breaking, enabling transformative task efficiency.
