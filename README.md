# school-handbook-qa-bot
AI Assistant that answers the parents repetitive questions from a school handbook (n8n+Gemini)
# School Handbook Q&A Bot

## Problem
Parents ask schools the same questions every day.

## Solution
An AI assistant that answers from the school handbook only. If the answer is not there, it says it doesn't know.

## How it works
1. Load the handbook PDF from Google Drive
2. Extract the text and split it into small pieces
3. Store the pieces in a vector store (searchable by meaning)
4. An AI agent searches the store and answers the parent's question

## Tools
n8n, Google Drive, Google Gemini, Simple Vector Store

## What I learned
“The assistant first searches the stored handbook pieces, then writes the answer from what it found.”
What the rule does: “I told it to answer only from the handbook, so it says ‘I don’t know’ instead of guessing.”
## Limits
- Vector store is temporary memory, so it resets if n8n restarts
- Works with text PDFs only
- Uses a fake practice handbook, no real school data

## Next steps
Urdu answers, a permanent database, WhatsApp
