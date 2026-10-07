# Prompt Budget Desk

A quick word-and-character estimate for packing a prompt into a context window you specify.

https://raeeskasim1.github.io/prompt-budget-desk/

## Try it

Paste English prose, code, and another language. Compare the word and character counts, and adjust budget and response reserve.

## How it works

This is an explicitly approximate planning tool, not a model tokenizer. The estimate is ceiling(Unicode code points / 4), a rough English-prose heuristic. It subtracts an answer reserve from a user-supplied budget. It does not track provider pricing, current model limits, system prompts, or chat-history overhead.

