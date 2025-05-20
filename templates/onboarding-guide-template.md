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

Welcome to **\[Company Name]**! Your onboarding is structured around two key goals:

* **Goal 1:** Start contributing code

* **Goal 2:** Prepare for on-call support

## 📅 Day 1 Task List

1. Get access to all tools

2. Set up your local environment

3. Complete a walkthrough of the codebase

4. Create your first PR

### ✅ Access Checklist

Please ensure you have access to all required tools and systems. Ask your onboarding buddy or manager if anything is missing.

<table class="dashdraft-table">
  <tbody>
    <tr class="dashdraft-table-row">
      <th class="dashdraft-table-header" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">System / Tool</p>
      </th>
      <th class="dashdraft-table-header" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">Notes / Links</p>
      </th>
    </tr>
    <tr class="dashdraft-table-row">
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">GitHub (Version Control)</p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">[Org Link]</p>
      </td>
    </tr>
    <tr class="dashdraft-table-row">
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">Slack (Communication)</p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">[Slack Workspace Invite]</p>
      </td>
    </tr>
    <tr class="dashdraft-table-row">
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">Google Workspace (Email)</p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">[Gmail / Calendar Access]</p>
      </td>
    </tr>
    <tr class="dashdraft-table-row">
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">Linear (Project Management)</p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">[Board Link]</p>
      </td>
    </tr>
    <tr class="dashdraft-table-row">
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">Joggr (Documentation)</p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">[Joggr Workspace Link]</p>
      </td>
    </tr>
    <tr class="dashdraft-table-row">
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">AWS / Vercel / GCP (Cloud)</p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">[Access Request / Console]</p>
      </td>
    </tr>
    <tr class="dashdraft-table-row">
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">Sentry / Datadog (Monitoring)</p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">[Monitoring Tool Link]</p>
      </td>
    </tr>
  </tbody>
</table>

### 🛠 Local Environment Setup

You’ll be working across multiple codebases. Start by cloning and running each one locally using the linked setup guides. Once your environments are running, move on to your first task and codebase walkthrough. If anything breaks, ask your onboarding buddy or use `#dev-support`.

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
        <p class="dashdraft-paragraph"><code class="dashdraft-code-inline">frontend-app</code></p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">Main user-facing web application</p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><a target="_blank" rel="noopener" class="dashdraft-link" href="#">View README</a></p>
      </td>
    </tr>
    <tr class="dashdraft-table-row">
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><code class="dashdraft-code-inline">api-service</code></p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">Core backend API</p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><a target="_blank" rel="noopener" class="dashdraft-link" href="#">View README</a></p>
      </td>
    </tr>
    <tr class="dashdraft-table-row">
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><code class="dashdraft-code-inline">auth-service</code></p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">Authentication &#x26; user sessions</p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><a target="_blank" rel="noopener" class="dashdraft-link" href="#">View README</a></p>
      </td>
    </tr>
    <tr class="dashdraft-table-row">
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><code class="dashdraft-code-inline">admin-dashboard</code></p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">Internal admin tool</p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><a target="_blank" rel="noopener" class="dashdraft-link" href="#">View README</a></p>
      </td>
    </tr>
  </tbody>
</table>

### 🚀 Make Your First Contribution

Now that your environments are running, it’s time to make your first change in one of the repos. Pick a small task — a bug fix, content tweak, or cleanup — and open a pull request. The goal is to get familiar with our workflow and how we work across repos.

### 📂 Supporting Guides (Per Repo)

Each repo has its own setup instructions, contribution process, and deployment flow. Use the links below to reference the right docs as you go:

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
        <p class="dashdraft-paragraph"><code class="dashdraft-code-inline">frontend-app</code></p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><a target="_blank" rel="noopener" class="dashdraft-link" href="#">View README</a></p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><a target="_blank" rel="noopener" class="dashdraft-link" href="#">View Guide</a></p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><a target="_blank" rel="noopener" class="dashdraft-link" href="#">View Deploy Guide</a></p>
      </td>
    </tr>
    <tr class="dashdraft-table-row">
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><code class="dashdraft-code-inline">api-service</code></p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><a target="_blank" rel="noopener" class="dashdraft-link" href="#">View README</a></p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><a target="_blank" rel="noopener" class="dashdraft-link" href="#">View Guide</a></p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><a target="_blank" rel="noopener" class="dashdraft-link" href="#">View Deploy Guide</a></p>
      </td>
    </tr>
    <tr class="dashdraft-table-row">
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><code class="dashdraft-code-inline">auth-service</code></p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><a target="_blank" rel="noopener" class="dashdraft-link" href="#">View README</a></p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><a target="_blank" rel="noopener" class="dashdraft-link" href="#">View Guide</a></p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><a target="_blank" rel="noopener" class="dashdraft-link" href="#">View Deploy Guide</a></p>
      </td>
    </tr>
    <tr class="dashdraft-table-row">
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><code class="dashdraft-code-inline">admin-dashboard</code></p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><a target="_blank" rel="noopener" class="dashdraft-link" href="#">View README</a></p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><a target="_blank" rel="noopener" class="dashdraft-link" href="#">View Guide</a></p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><a target="_blank" rel="noopener" class="dashdraft-link" href="#">View Deploy Guide</a></p>
      </td>
    </tr>
  </tbody>
</table>

> 📌 Not all deploys are the same — some use CI/CD, some are manual, some require approvals. Always check the repo-specific deployment guide before shipping anything.

### 🧭 Shared References (Global)

If you need broader context while working:

* 🧱 [Architecture Overview](#)

* 🧑‍🎨 [Code Style Guide](#)

> 💬 Questions? Reach out to your onboarding buddy or post in `#dev-support`.

## 📅 Day 2 Task List

### 🔄 Working in Our Development Workflow

With your first PR complete, it’s time to get familiar with how we work day-to-day.

<table class="dashdraft-table">
  <tbody>
    <tr class="dashdraft-table-row">
      <th class="dashdraft-table-header" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">Workflow Guide</p>
      </th>
      <th class="dashdraft-table-header" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">Description</p>
      </th>
    </tr>
    <tr class="dashdraft-table-row">
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><a target="_blank" rel="noopener" class="dashdraft-link" href="#">Sprint &#x26; Issue Workflow</a></p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">How we plan, assign, and track work</p>
      </td>
    </tr>
    <tr class="dashdraft-table-row">
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><a target="_blank" rel="noopener" class="dashdraft-link" href="#">Git Workflow</a></p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">Branching strategy and release process</p>
      </td>
    </tr>
    <tr class="dashdraft-table-row">
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><a target="_blank" rel="noopener" class="dashdraft-link" href="#">Testing &#x26; Review Guide</a></p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">Writing tests and submitting high-quality PRs</p>
      </td>
    </tr>
    <tr class="dashdraft-table-row">
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><a target="_blank" rel="noopener" class="dashdraft-link" href="#">Deployment Guide</a></p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">How to ship code to staging/production</p>
      </td>
    </tr>
  </tbody>
</table>

### 🔔 Preparing for On-Call Support

Once you're contributing confidently, the next goal is to be ready to support the systems you work on.

<table class="dashdraft-table">
  <tbody>
    <tr class="dashdraft-table-row">
      <th class="dashdraft-table-header" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">On-Call Preparation</p>
      </th>
      <th class="dashdraft-table-header" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">Description</p>
      </th>
    </tr>
    <tr class="dashdraft-table-row">
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><a target="_blank" rel="noopener" class="dashdraft-link" href="#">Incident Response Playbook</a></p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">How we handle outages and escalations</p>
      </td>
    </tr>
    <tr class="dashdraft-table-row">
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><a target="_blank" rel="noopener" class="dashdraft-link" href="#">Logging &#x26; Monitoring Guide</a></p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">Tools for debugging and observability</p>
      </td>
    </tr>
    <tr class="dashdraft-table-row">
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><a target="_blank" rel="noopener" class="dashdraft-link" href="#">Debugging &#x26; Access Guide</a></p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">Dashboards, logs, and tools you’ll use</p>
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
