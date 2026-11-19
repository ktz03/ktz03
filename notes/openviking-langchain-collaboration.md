# OpenViking + LangChain: preserving conversation history

**Project:** OpenViking · **Area:** agent memory and integrations · **Outcome:** merged upstream

[PR #6275](https://github.com/volcengine/OpenViking/pull/6275) · [Coauthor credit](https://github.com/volcengine/OpenViking/commit/b1d0fa51ef253716fdec819615918352e97dfd41)

## Problem

Conversation text, message roles and completed tool-call information could be lost or misclassified when recording and restoring history.

## Collaboration

The upstream PR, opened by [@ehz0ah](https://github.com/ehz0ah), consolidated multiple fixes to preserve text, role handling and tool history. The linked commit records ktz03 as a coauthor. The original PR author and contributors retain their respective credit.

## Evidence and scope

The PR contains its own test results, version details and coverage limits. This case describes a collaborative merged change, rather than attributing the entire PR to one person.
