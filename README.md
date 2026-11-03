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
I learned how to store data in a vector data base and how to splits the text into the chunks and after it I adjoined the chat part how an answered is got how embed the AI model .By system message I restricted it to the given data ,it doesn't allow it to generate it's own answers.Then I explored the context engineering.

## Limits
- Vector store is temporary memory, so it resets if n8n restarts
- Works with text PDFs only
- Uses a fake practice handbook, no real school data

## Next steps
Urdu answers, a permanent database, WhatsApp
