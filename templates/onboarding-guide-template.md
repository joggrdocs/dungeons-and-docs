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
## 🧭 Developer Onboarding Guide

Welcome to **\[Company Name]**! This guide will help you get productive quickly. You’ll start writing code and learn how to support production systems as part of your onboarding journey.

* **Goal 1 – Start Writing Code**: Get familiar with our repositories, development tools, and contribution workflow.

* **Goal 2 – Prepare for On-Call Support**: Learn how to monitor, debug, and support the systems you’ll be working on.

## 📅 Day 1: First Contribution

### 🔐 Access Checklist

Make sure you have access to the following systems. Ask your onboarding buddy if anything’s missing.

<table class="dashdraft-table">
  <tbody>
    <tr class="dashdraft-table-row">
      <th class="dashdraft-table-header" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">Tool</p>
      </th>
      <th class="dashdraft-table-header" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">Description</p>
      </th>
    </tr>
    <tr class="dashdraft-table-row">
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><strong class="dashdraft-bold">GitHub</strong></p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">Code hosting &#x26; version control</p>
      </td>
    </tr>
    <tr class="dashdraft-table-row">
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><strong class="dashdraft-bold">Slack</strong></p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">Team communication</p>
      </td>
    </tr>
    <tr class="dashdraft-table-row">
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><strong class="dashdraft-bold">Google Workspace</strong></p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">Email &#x26; calendar access</p>
      </td>
    </tr>
    <tr class="dashdraft-table-row">
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><strong class="dashdraft-bold">Linear</strong></p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">Project &#x26; issue tracking</p>
      </td>
    </tr>
    <tr class="dashdraft-table-row">
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><strong class="dashdraft-bold">Joggr</strong></p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">Internal documentation</p>
      </td>
    </tr>
    <tr class="dashdraft-table-row">
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><strong class="dashdraft-bold">AWS / Vercel / GCP</strong></p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">Cloud infrastructure &#x26; deployment</p>
      </td>
    </tr>
    <tr class="dashdraft-table-row">
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><strong class="dashdraft-bold">Sentry / Datadog</strong></p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">Monitoring &#x26; observability</p>
      </td>
    </tr>
  </tbody>
</table>

### 🛠 Local Environment Setup

You’ll be working across multiple codebases. Start by cloning and running each repo locally using its setup guide:

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
        <p class="dashdraft-paragraph">React-based UI</p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">View README</p>
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
        <p class="dashdraft-paragraph">View README</p>
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
        <p class="dashdraft-paragraph">View README</p>
      </td>
    </tr>
  </tbody>
</table>

### 🚀 Make Your First Contribution

Now that you’re set up, make your first real change. It doesn’t need to be big—just meaningful. Open a pull request (PR) and request a review from your buddy or tech lead.

<table class="dashdraft-table">
  <tbody>
    <tr class="dashdraft-table-row">
      <th class="dashdraft-table-header" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">Repo</p>
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
        <p class="dashdraft-paragraph"><a target="_blank" rel="noopener noreferrer" class="dashdraft-link" href="https://github.com/joggrdocs/dungeons-and-docs/blob/main/templates/project/contribution-guidelines.md">Guide</a></p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><a target="_blank" rel="noopener noreferrer" class="dashdraft-link" href="https://github.com/joggrdocs/dungeons-and-docs/blob/main/templates/project/deployment-guide.md">Deploy</a></p>
      </td>
    </tr>
    <tr class="dashdraft-table-row">
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><code class="dashdraft-code-inline">backend</code></p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><a target="_blank" rel="noopener noreferrer" class="dashdraft-link" href="https://github.com/joggrdocs/dungeons-and-docs/blob/main/templates/project/contribution-guidelines.md">Guide</a></p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><a target="_blank" rel="noopener noreferrer" class="dashdraft-link" href="https://github.com/joggrdocs/dungeons-and-docs/blob/main/templates/project/deployment-guide.md">Deploy</a></p>
      </td>
    </tr>
    <tr class="dashdraft-table-row">
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><code class="dashdraft-code-inline">infra</code></p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><a target="_blank" rel="noopener noreferrer" class="dashdraft-link" href="https://github.com/joggrdocs/dungeons-and-docs/blob/main/templates/project/contribution-guidelines.md">Guide</a></p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><a target="_blank" rel="noopener noreferrer" class="dashdraft-link" href="https://github.com/joggrdocs/dungeons-and-docs/blob/main/templates/project/deployment-guide.md">Deploy</a></p>
      </td>
    </tr>
  </tbody>
</table>

## 📅 Day 2: Contribute with Confidence

### 📚 Engineering Essentials

Broaden your understanding of our codebase and team structure

<table class="dashdraft-table">
  <tbody>
    <tr class="dashdraft-table-row">
      <th class="dashdraft-table-header" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">Guide</p>
      </th>
      <th class="dashdraft-table-header" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">Description</p>
      </th>
    </tr>
    <tr class="dashdraft-table-row">
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><span data-name="bricks" class="dashdraft-emoji" data-type="emoji">🧱</span> <a target="_blank" rel="noopener noreferrer" class="dashdraft-link" href="https://github.com/joggrdocs/dungeons-and-docs/blob/main/templates/architecture/service-architecture.md">Architecture Overview</a></p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">System diagrams &#x26; key technical decisions</p>
      </td>
    </tr>
    <tr class="dashdraft-table-row">
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><span data-name="artist" class="dashdraft-emoji" data-type="emoji">🧑‍🎨</span> <a target="_blank" rel="noopener noreferrer" class="dashdraft-link" href="https://github.com/joggrdocs/dungeons-and-docs/blob/main/templates/standards/code-style.md">Code Style Guide</a></p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">Formatting, linting, naming conventions</p>
      </td>
    </tr>
    <tr class="dashdraft-table-row">
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><span data-name="package" class="dashdraft-emoji" data-type="emoji">📦</span> <a target="_blank" rel="noopener noreferrer" class="dashdraft-link" href="https://github.com/joggrdocs/dungeons-and-docs/blob/main/templates/team/product-overview.md">Product Overview</a></p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">What we build and who it’s for</p>
      </td>
    </tr>
    <tr class="dashdraft-table-row">
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><span data-name="busts_in_silhouette" class="dashdraft-emoji" data-type="emoji">👥</span> <a target="_blank" rel="noopener noreferrer" class="dashdraft-link" href="https://github.com/joggrdocs/dungeons-and-docs/blob/main/templates/team/team-overview.md">Team Overview</a></p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">Org structure and team contacts</p>
      </td>
    </tr>
  </tbody>
</table>

### 🔄 Development Workflow

Learn how we collaborate, plan, and ship code effectively:

<table class="dashdraft-table">
  <tbody>
    <tr class="dashdraft-table-row">
      <th class="dashdraft-table-header" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">Topic</p>
      </th>
      <th class="dashdraft-table-header" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">Description</p>
      </th>
    </tr>
    <tr class="dashdraft-table-row">
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><a target="_blank" rel="noopener noreferrer" class="dashdraft-link" href="https://github.com/joggrdocs/dungeons-and-docs/blob/main/templates/standards/sprint-and-issue-workflow.md">Sprint &#x26; Issue Workflow</a></p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">How we plan, assign, and track work</p>
      </td>
    </tr>
    <tr class="dashdraft-table-row">
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><a target="_blank" rel="noopener noreferrer" class="dashdraft-link" href="https://github.com/joggrdocs/dungeons-and-docs/blob/main/templates/standards/software-development.md">Software Development Process</a></p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">From idea to feature delivery</p>
      </td>
    </tr>
    <tr class="dashdraft-table-row">
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><a target="_blank" rel="noopener noreferrer" class="dashdraft-link" href="https://github.com/joggrdocs/dungeons-and-docs/blob/main/templates/standards/meeting-ceremonies.md">Meeting &#x26; Team Ceremonies</a></p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">Standups, sprint planning, retros, etc.</p>
      </td>
    </tr>
  </tbody>
</table>

### 🔔 On-Call Ready

As you ramp up, you’ll also begin learning how to support the systems you contribute to:

<table class="dashdraft-table">
  <tbody>
    <tr class="dashdraft-table-row">
      <th class="dashdraft-table-header" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">Guide</p>
      </th>
      <th class="dashdraft-table-header" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">Description</p>
      </th>
    </tr>
    <tr class="dashdraft-table-row">
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><a target="_blank" rel="noopener noreferrer" class="dashdraft-link" href="https://github.com/joggrdocs/dungeons-and-docs/blob/main/templates/standards/incident-management.md">Incident Response Playbook</a></p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">How we handle outages and escalations</p>
      </td>
    </tr>
    <tr class="dashdraft-table-row">
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><a target="_blank" rel="noopener noreferrer" class="dashdraft-link" href="https://github.com/joggrdocs/dungeons-and-docs/blob/main/templates/standards/logging-and-monitoring.md">Logging &#x26; Monitoring Guide</a></p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">Observability tools (logs, metrics, alerts)</p>
      </td>
    </tr>
  </tbody>
</table>

<!-- @joggr:editLink(fcd57b32-dd26-4e18-a4ae-397acf560633):start -->
---
<a href="https://app.joggr.io/app/documents/fcd57b32-dd26-4e18-a4ae-397acf560633/edit">
  <img src="https://cdn.joggr.io/assets/static/badges/joggr-document-edit.svg?did=fcd57b32-dd26-4e18-a4ae-397acf560633" alt="Edit doc on Joggr" />
</a>
<!-- @joggr:editLink(fcd57b32-dd26-4e18-a4ae-397acf560633):end -->
