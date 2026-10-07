# Prompt Budget Desk

A quick word-and-character estimate for packing a prompt into a context window you specify.

## Run

Open `index.html` in a modern browser. HTML, CSS, and JavaScript are all in that file. No server, packages, internet connection, API key, build step, or downloaded model is required.

## Try it

Paste English prose, code, and another language. Compare the word and character counts, and adjust budget and response reserve.

## How it works

This is an explicitly approximate planning tool, not a model tokenizer. The estimate is ceiling(Unicode code points / 4), a rough English-prose heuristic. It subtracts an answer reserve from a user-supplied budget. It does not track provider pricing, current model limits, system prompts, or chat-history overhead.

