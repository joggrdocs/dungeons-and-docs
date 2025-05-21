<!--@@joggrdoc@@-->
<!-- @joggr:version(v2):end -->
<!-- @joggr:warning:start -->
<!-- 
  _   _   _    __        __     _      ____    _   _   ___   _   _    ____     _   _   _ 
 | | | | | |   \ \      / /    / \    |  _ \  | \ | | |_ _| | \ | |  / ___|   | | | | | |
 | | | | | |    \ \ /\ / /    / _ \   | |_) | |  \| |  | |  |  \| | | |  _    | | | | | |
 |_| |_| |_|     \ V  V /    / ___ \  |  _ <  | |\  |  | |  | |\  | | |_| |   |_| |_| |_|
 (_) (_) (_)      \_/\_/    /_/   \_\ |_| \_\ |_| \_| |___| |_| \_|  \____|   (_) (_) (_)
                                                              
This document is managed by Joggr. Editing this document could break Joggr's core features, i.e. our 
ability to auto-maintain this document. Please use the Joggr editor to edit this document 
(link at bottom of the page).
-->
<!-- @joggr:warning:end -->
# 🧭 Developer Onboarding Guide

Welcome to **\[Company Name]**! Your onboarding is structured around two key goals.

**Goal 1: Start writing code**: Get familiar with our repositories, development tools, and contribution workflow.

**Goal 2: Prepare for on-call support**: Learn how to monitor, debug, and support the systems you’ll be working on.

### 📅 Day 1 Tasks

1. ✅ Get access to all tools and systems

2. 🛠 Set up your local dev environment

3. 🧭 Walk through the codebase

4. 🚀 Open your first PR

#### ✅ Access Checklist

Please ensure you have access to all required tools and systems. Ask your onboarding buddy or manager if anything is missing.

**Core Tools**

* [GitHub](#) – Code hosting & version control

* [Slack](#) – Team communication

* [Google Workspace](#) – Gmail & Calendar access

* [Linear](#) – Project & issue tracking

* [Joggr](#) – Internal documentation

* [AWS / Vercel / GCP](#) – Deployment & cloud infra

* [Sentry / Datadog](#) – Monitoring and observability

#### 🛠 Local Environment Setup

You’ll be working across multiple codebases. Start by cloning and running each one locally using the linked setup guides. If anything breaks, ask your onboarding buddy or post in `#[enter-slack-channel]`.

<table class="dashdraft-table">
  <tbody>
    <tr class="dashdraft-table-row">
      <th class="dashdraft-table-header" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">Codebase</p>
      </th>
      <th class="dashdraft-table-header" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">Description</p>
      </th>
      <th class="dashdraft-table-header" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">Setup Guide</p>
      </th>
    </tr>
    <tr class="dashdraft-table-row">
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><code class="dashdraft-code-inline">frontend</code></p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">Our React-based UI</p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><a target="_blank" rel="noopener" class="dashdraft-link" href="#">View README</a></p>
      </td>
    </tr>
    <tr class="dashdraft-table-row">
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><code class="dashdraft-code-inline">backend</code></p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">API and core logic</p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><a target="_blank" rel="noopener" class="dashdraft-link" href="#">View README</a></p>
      </td>
    </tr>
    <tr class="dashdraft-table-row">
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><code class="dashdraft-code-inline">infra</code></p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">Infrastructure-as-code</p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><a target="_blank" rel="noopener" class="dashdraft-link" href="#">View README</a></p>
      </td>
    </tr>
  </tbody>
</table>

#### 🚀 Make Your First Contribution

Now that your environment is set up, it’s time to make your first real change. It doesn’t have to be big, just something that goes through the full workflow. Open a pull request (PR) and request a review from your onboarding buddy or tech lead. Use the links below to follow each repo’s contribution guidelines and PR process.

<table class="dashdraft-table">
  <tbody>
    <tr class="dashdraft-table-row">
      <th class="dashdraft-table-header" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">Repo</p>
      </th>
      <th class="dashdraft-table-header" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">README / Setup</p>
      </th>
      <th class="dashdraft-table-header" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">CONTRIBUTING.md</p>
      </th>
      <th class="dashdraft-table-header" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">Deployment Guide</p>
      </th>
    </tr>
    <tr class="dashdraft-table-row">
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><code class="dashdraft-code-inline">frontend</code></p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><a target="_blank" rel="noopener" class="dashdraft-link" href="#">README</a></p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><a target="_blank" rel="noopener" class="dashdraft-link" href="#">Guide</a></p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><a target="_blank" rel="noopener" class="dashdraft-link" href="#">Deploy</a></p>
      </td>
    </tr>
    <tr class="dashdraft-table-row">
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><code class="dashdraft-code-inline">backend</code></p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><a target="_blank" rel="noopener" class="dashdraft-link" href="#">README</a></p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><a target="_blank" rel="noopener" class="dashdraft-link" href="#">Guide</a></p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><a target="_blank" rel="noopener" class="dashdraft-link" href="#">Deploy</a></p>
      </td>
    </tr>
    <tr class="dashdraft-table-row">
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><code class="dashdraft-code-inline">infra</code></p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><a target="_blank" rel="noopener" class="dashdraft-link" href="#">README</a></p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><a target="_blank" rel="noopener" class="dashdraft-link" href="#">Guide</a></p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><a target="_blank" rel="noopener" class="dashdraft-link" href="#">Deploy</a></p>
      </td>
    </tr>
  </tbody>
</table>

### 📅 **Day 2: Contributing with Confidence**

With your environment ready and your first PR in motion, today is all about building fluency in how we code, collaborate, and support production systems.

#### 📚 Reference Hub

Use these guides to get broader context on the code, systems, and people you’ll be working with:

* 🧱 [**Architecture Overview**](#link-to-architecture-overview) – High-level system diagrams & key decisions

* 🧑‍🎨 [**Code Style Guide**](#link-to-code-style-guide) – Linting, formatting, naming conventions

* 📦 [**Product Overview**](#link-to-product-overview) – What we build and who it’s for

* 👥 [**Team Overview**](#link-to-team-overview) – Who’s who, teams, and org structure

***

#### 🔄 Working in Our Development Workflow

Get familiar with how we work day-to-day—from planning and standups to code delivery:

* [**Sprint & Issue Workflow**](#link-to-sprint-workflow) – How we plan, assign, and track work

* [**Software Development Process**](#link-to-dev-process) – How features move from idea to development to production

* [**Meeting & Team Ceremonies**](#link-to-meeting-ceremonies) – Standups, sprint planning, retros, and how/when we communicate as a team

#### 🔔 Getting On-Call Ready

As you grow more comfortable, it’s important to start preparing for production support responsibilities. These docs walk you through the tools and processes we use:

* [**Incident Response Playbook**](#link-to-incident-playbook) – How we handle outages and escalations

* [**Logging & Monitoring Guide**](#link-to-logging-monitoring-guide) – Tools for observability and debugging

* [**Debugging & Access Guide**](#link-to-debugging-access-guide) – Dashboards, logs, and tools you’ll use

<!-- @joggr:editLink(fcd57b32-dd26-4e18-a4ae-397acf560633):start -->
---
<a href="https://app.joggr.io/app/documents/fcd57b32-dd26-4e18-a4ae-397acf560633/edit">
  <img src="https://cdn.joggr.io/assets/static/badges/joggr-document-edit.svg?did=fcd57b32-dd26-4e18-a4ae-397acf560633" alt="Edit doc on Joggr" />
</a>
<!-- @joggr:editLink(fcd57b32-dd26-4e18-a4ae-397acf560633):end -->
