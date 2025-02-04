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
## 📜 Our Three Core Rules for Documentation

1. **Anonymity** – Docs reflect team knowledge, not individual authors.

2. **Clarity** – The name and summary should make the purpose obvious.

3. **Discoverability** – Docs live where you'd logically expect them.

Following these rules means:

* 🚀 **Faster dev work** – No more getting stuck in question purgatory.

* 🛹 **Smoother onboarding** – New devs ramp up without roadblocks.

* 🔮 **Future-you will thank you** – When debugging your own cryptic code, good docs are a lifesaver.

## What You'll Learn

Please read this document, and apply it to your documentation writing! In this document, you will find all of the following:

<table class="dashdraft-table">
  <tbody>
    <tr class="dashdraft-table-row">
      <th class="dashdraft-table-header" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">Section</p>
      </th>
      <th class="dashdraft-table-header" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">What You'll Learn</p>
      </th>
    </tr>
    <tr class="dashdraft-table-row">
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">Types of Documentation</p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">You'll learn about how we define certain types of documentation.</p>
      </td>
    </tr>
    <tr class="dashdraft-table-row">
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">When to Create JoggrDocs</p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">You'll learn when we expect developers to create certain types of documentation.</p>
      </td>
    </tr>
    <tr class="dashdraft-table-row">
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">How to Create JoggrDocs</p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">You'll learn what we expect when you create documentation (e.g. naming conventions)</p>
      </td>
    </tr>
    <tr class="dashdraft-table-row">
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">Where to Save Documentation</p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">You'll learn where to save documentation in Joggr &#x26; GitHub.</p>
      </td>
    </tr>
  </tbody>
</table>

## Software Development Process

It's important to understand that documentation is a continuous part of our process and a key component of our Software Development Process. This diagram provides an overview of how documentation is integrated into our development process.

```mermaid
graph LR;

    %% Entities
    prd(Create PRD);
    rfc(Create RFC);
    code(Write Code);
    openPR(Open PR);
    part4A(Update/Create HTTP APIs);
    part4B(Update/Create Guides);
    part4C(Update/Create Docs);
    done(Done);

    %% Flow
    prd --> rfc;
    rfc --> code;
    code --> openPR;
    openPR -- "Modify a HTTP API?" --> part4A;
    openPR -- "Modify a standard process?" --> part4B;
    openPR -- "Modify a complex part of our codebase?" --> part4C;
    part4A --> done;
    part4B --> done;
    part4C --> done;

  subgraph "Planning Phase"
    prd;
    rfc;
  end;

  subgraph "Coding Phase"
    code;
    openPR;
  end;

  subgraph "Code Review Phase"
    part4A;
    part4B;
    part4C;
  end;
```

### Types of Documentation

<table class="dashdraft-table">
  <tbody>
    <tr class="dashdraft-table-row">
      <th class="dashdraft-table-header" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">Category</p>
      </th>
      <th class="dashdraft-table-header" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">Description</p>
      </th>
    </tr>
    <tr class="dashdraft-table-row">
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">Request for Comment (RFC)</p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">RFCs help developers think through a design or feature before coding. Use RFCs to think through a design &#x26; get feedback from the team.</p>
      </td>
    </tr>
    <tr class="dashdraft-table-row">
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">Architecture</p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">An architecture document shows the architecture of the system &#x26; how different components interact.</p>
      </td>
    </tr>
    <tr class="dashdraft-table-row">
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">Guides</p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">A guide shows developers how to complete a task (e.g. how to deploy).</p>
      </td>
    </tr>
    <tr class="dashdraft-table-row">
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">Walkthroughs</p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">A walkthrough shows developers how something works, often "walking" a developer through the code (i.e. How Authentication Works).</p>
      </td>
    </tr>
  </tbody>
</table>

### Joggr Directory Structure

Below is our Directory Structure in Joggr. Please make sure to save all documents to the correct position.

<table class="dashdraft-table">
  <tbody>
    <tr class="dashdraft-table-row">
      <th class="dashdraft-table-header" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">Folder</p>
      </th>
      <th class="dashdraft-table-header" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">Description</p>
      </th>
    </tr>
    <tr class="dashdraft-table-row">
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><code class="dashdraft-code-inline">Overview</code></p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">Describe in 1-2 sentences what documentation should be saved to this folder.</p>
      </td>
    </tr>
    <tr class="dashdraft-table-row">
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><code class="dashdraft-code-inline">Standards</code></p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">Describe in 1-2 sentences what documentation should be saved to this folder.</p>
      </td>
    </tr>
    <tr class="dashdraft-table-row">
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><code class="dashdraft-code-inline">Architecture</code></p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">Describe in 1-2 sentences what documentation should be saved to this folder.</p>
      </td>
    </tr>
    <tr class="dashdraft-table-row">
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><code class="dashdraft-code-inline">Frontend</code></p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">Describe in 1-2 sentences what documentation should be saved to this folder.</p>
      </td>
    </tr>
    <tr class="dashdraft-table-row">
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><code class="dashdraft-code-inline">Backend</code></p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">Describe in 1-2 sentences what documentation should be saved to this folder.</p>
      </td>
    </tr>
  </tbody>
</table>

### GitHub Directory Structure

Below is our approach to storing docs in GitHub. We have two places to store docs in GitHub:

<table class="dashdraft-table">
  <tbody>
    <tr class="dashdraft-table-row">
      <th class="dashdraft-table-header" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">Area</p>
      </th>
      <th class="dashdraft-table-header" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">Description</p>
      </th>
    </tr>
    <tr class="dashdraft-table-row">
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><a target="_blank" rel="noopener noreferrer" class="dashdraft-link" href="github.com">Tech-Docs Repository</a></p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">This repository holds documentation that does not make sense to put in a specific repository (i.e. Code Review Standards).</p>
      </td>
    </tr>
    <tr class="dashdraft-table-row">
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><code class="dashdraft-code-inline">/docs</code> directory in a code repositories</p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">In every repository, we should have a <code class="dashdraft-code-inline">/docs</code> directory. If you are documenting something where it's obvious it should be saved in that repository, save it to the <code class="dashdraft-code-inline">/docs</code> folder.</p>
      </td>
    </tr>
  </tbody>
</table>

> \[!NOTE]
>
> The Tech Docs Repostitory's file tree **should** mirror our Joggr file tree.

### When to Create JoggrDocs

We expect that software developers create documentation based on the following:

<table class="dashdraft-table">
  <tbody>
    <tr class="dashdraft-table-row">
      <th class="dashdraft-table-header" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">RFC</p>
      </th>
      <th class="dashdraft-table-header" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">Arch.</p>
      </th>
      <th class="dashdraft-table-header" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">Guides</p>
      </th>
      <th class="dashdraft-table-header" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">Walkthroughs</p>
      </th>
    </tr>
    <tr class="dashdraft-table-row">
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><strong class="dashdraft-bold">MUST</strong> be created after approving the PRD and before starting development.</p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><strong class="dashdraft-bold">MUST</strong> create an architecture diagram for any new large project.</p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><strong class="dashdraft-bold">MUST</strong> be created or updated when a new standard process is introduced or an existing one is updated.</p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><strong class="dashdraft-bold">MUST</strong> be created when the team starts asking lots of questions about a certain part of our codebase (e.g. how does authentication work)</p>
      </td>
    </tr>
  </tbody>
</table>

### How to Create JoggrDocs

We expect software developers to follow these standards when creating documentation.

<table class="dashdraft-table">
  <tbody>
    <tr class="dashdraft-table-row">
      <th class="dashdraft-table-header" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">RFC</p>
      </th>
      <th class="dashdraft-table-header" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">Arch.</p>
      </th>
      <th class="dashdraft-table-header" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">Guides</p>
      </th>
      <th class="dashdraft-table-header" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">Walkthroughs</p>
      </th>
    </tr>
    <tr class="dashdraft-table-row">
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><strong class="dashdraft-bold">MUST</strong> use the RFC Template</p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><strong class="dashdraft-bold">MUST </strong>include a diagram</p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><strong class="dashdraft-bold">MUST</strong> use the How-To Guide template</p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><strong class="dashdraft-bold">MUST </strong>reference code examples where possible.</p>
      </td>
    </tr>
  </tbody>
</table>

<!-- @joggr:editLink(284ccfba-f508-4d64-aaf4-cef948ae6e58):start -->
---
<a href="https://app.joggr.io/app/documents/284ccfba-f508-4d64-aaf4-cef948ae6e58/edit">
  <img src="https://cdn.joggr.io/assets/static/badges/joggr-document-edit.svg?did=284ccfba-f508-4d64-aaf4-cef948ae6e58" alt="Edit doc on Joggr" />
</a>
<!-- @joggr:editLink(284ccfba-f508-4d64-aaf4-cef948ae6e58):end -->
