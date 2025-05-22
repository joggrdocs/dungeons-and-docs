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

Welcome to **\[Company Name]**! This guide will help you get productive quickly.

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

### 📚 Engineering Essentials

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
        <p class="dashdraft-paragraph">Gain a high-level understanding of how our systems are structured. This guide covers key components, service interactions, &#x26; data flow.</p>
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

### 🚀 Make Your First Contribution

Now that you’re set up, make your first real change. It doesn’t need to be big—just meaningful. Open a pull request (PR) and request a review from your buddy or tech lead.

<table class="dashdraft-table">
  <tbody>
    <tr class="dashdraft-table-row">
      <th class="dashdraft-table-header" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">Repo</p>
      </th>
      <th class="dashdraft-table-header" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">README</p>
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

<!-- @joggr:editLink(d5a30697-c4af-4404-ad58-83edf6c65b69):start -->
---
<a href="https://app.joggr.io/app/documents/d5a30697-c4af-4404-ad58-83edf6c65b69/edit">
  <img src="https://cdn.joggr.io/assets/static/badges/joggr-document-edit.svg?did=d5a30697-c4af-4404-ad58-83edf6c65b69" alt="Edit doc on Joggr" />
</a>
<!-- @joggr:editLink(d5a30697-c4af-4404-ad58-83edf6c65b69):end -->
