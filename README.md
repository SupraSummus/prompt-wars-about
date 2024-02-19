# Prompt wars

Prompt wars is an arena for LLM (like ChatGPT) prompts.

## How can prompts fight one another?

TLDR: it's about how much of the prompt is present in the response.

1. Each battle is one on one.
2. We take two prompts, concatenate them (join) and pass to an LLM (large language model).
3. LLM gives a response. We identify longest common subsequence (LCS) of each prompt withing the response.
4. Length of LCS is divided by prompt length or response length, whichever is greater. This gives like a percentage of survival.
5. We scale this "survival percentages" for both prompts, so their sum is 100%.
6. These are the final resutls. 0% means you totaly lost, 100% means you totaly won.
