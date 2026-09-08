---
document_id: SEC-SYSTEM-RETRIEVAL-001
title: GitHub KB-First Mandatory Retrieval Policy
version: 1.0
status: Active
owner: KB Owner
scope: One Bangkok / Security Emergency Procedures
repository: jimmytherocket3-star/security-knowledge-base
updated: 2026-09-08
---

# GitHub KB-First Mandatory Retrieval Policy

## Purpose

Define the approved retrieval priority for AI answering questions related to One Bangkok, Security Emergency Procedures, internal emergency codes, locations/buildings, loading points, contacts, management codes, and other knowledge maintained in this repository.

## Mandatory Retrieval Rule

For any question that is reasonably related to One Bangkok or this Security Knowledge Base, the AI must use `jimmytherocket3-star/security-knowledge-base` as the primary knowledge source and retrieve/search the relevant approved GitHub KB content before producing a factual answer whenever GitHub access is available.

This rule is intended to apply even when the question is asked in a new chat and the previous conversation context is unavailable.

## Retrieval Order

1. Identify whether the question is within One Bangkok / Security KB scope.
2. Search or fetch the relevant content from `jimmytherocket3-star/security-knowledge-base`.
3. Prefer the latest approved / Active KB knowledge relevant to the question.
4. If the answer is present in the KB, answer from the KB and preserve approved terminology.
5. If the answer is not present or is incomplete, state that it is a Knowledge Gap / unconfirmed rather than guessing.
6. Use external sources only when the user explicitly requests external research/verification or when clearly separated from internal KB knowledge.

## Examples of KB-First Questions

- `One00 คือใคร?`
- `Loading 4 เป็นของอาคารอะไร?`
- `Code Sierra คืออะไร?`
- `Code 3 ต้องทำอะไร?`
- `DCC คืออะไร?`
- `เบอร์ SOC คืออะไร?`
- `Tower 5 อยู่ส่วนไหน?`
- Questions about One Bangkok buildings, zones, emergency procedures, contacts, roles, terminology, or approved operational references.

## New-Chat Behavior

When a new conversation does not contain prior KB context, lack of chat history must not by itself be treated as evidence that the KB has no answer. If GitHub access is available, the AI should retrieve the KB before saying that the information is unavailable or unconfirmed.

## Source Priority

Within KB scope, use this priority:

`Latest Approved/Active KB → Approved Reference KB → Knowledge Gap → External source (only when requested/appropriate)`

Draft or source-specific material must not silently override a later approved canonical definition.

## AI Guardrails

1. Never guess an internal One Bangkok fact when the KB can be searched.
2. Never claim that a fact is absent from the KB without attempting relevant retrieval when GitHub access is available.
3. Do not substitute general web knowledge for approved internal KB knowledge.
4. Preserve distinctions between Active SOP, Reference, Draft, time-bound schedule, drill scenario, and source-specific material.
5. If GitHub access is unavailable in a particular chat/session, say that the KB could not be retrieved in that session rather than pretending it was checked.
6. This repository policy expresses the KB Owner's approved retrieval behavior; actual cross-chat enforcement still depends on the ChatGPT session having access to the GitHub connector/repository and receiving or discovering this policy.
7. All KB modifications remain subject to the existing Proposal → KB Owner Review → Approval workflow.

## Change Log

- v1.0 — 2026-09-08 — Created after explicit KB Owner approval. Establishes GitHub KB-first retrieval as the primary answering policy for One Bangkok / Security KB questions, including new-chat behavior where GitHub access is available.
