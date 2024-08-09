## Overview

We live by three core rules with our documentation:

1. **You cannot tell who wrote the document, only that someone on the team did.**

2. **You can easily grok what a document is based on its name and summary.**

3. **You automatically know where you should be able to find a document based on what you are looking for (aka it's in the right directory).**

If we follow these 3 core rules and our standards it will allow our team to:

* 🚀 **Move faster** - great docs help devs work independently and not get bogged down in question hell.

* 🛹 **Onboard faster** - when you have great docs new devs can easily get up to speed and start contributing.

* 🔮 **Be kind to your *Future Self*** - you will eventually write super complex code and you won't remember why. If you write great docs you can thank your past self for helping you untangle whatever spaghetti is in front of you.

## What You'll Learn

Please read this document, and apply it to your documentation writing! In this document, you will find all of the following:

<table class="dashdraft-table"><tbody><tr class="dashdraft-table-row"><th class="dashdraft-table-header" colspan="1" rowspan="1"><p class="dashdraft-paragraph">Section</p></th><th class="dashdraft-table-header" colspan="1" rowspan="1"><p class="dashdraft-paragraph">What You'll Learn</p></th></tr><tr class="dashdraft-table-row"><td class="dashdraft-table-cell" colspan="1" rowspan="1"><p class="dashdraft-paragraph">Types of Documentation</p></td><td class="dashdraft-table-cell" colspan="1" rowspan="1"><p class="dashdraft-paragraph">You'll learn about how we define certain types of documentation.</p></td></tr><tr class="dashdraft-table-row"><td class="dashdraft-table-cell" colspan="1" rowspan="1"><p class="dashdraft-paragraph">When to Create JoggrDocs</p></td><td class="dashdraft-table-cell" colspan="1" rowspan="1"><p class="dashdraft-paragraph">You'll learn when we expect developers to create certain types of documentation.</p></td></tr><tr class="dashdraft-table-row"><td class="dashdraft-table-cell" colspan="1" rowspan="1"><p class="dashdraft-paragraph">How to Create JoggrDocs</p></td><td class="dashdraft-table-cell" colspan="1" rowspan="1"><p class="dashdraft-paragraph">You'll learn what we expect when you create documentation (e.g. naming conventions)</p></td></tr><tr class="dashdraft-table-row"><td class="dashdraft-table-cell" colspan="1" rowspan="1"><p class="dashdraft-paragraph">Where to Save Documentation</p></td><td class="dashdraft-table-cell" colspan="1" rowspan="1"><p class="dashdraft-paragraph">You'll learn where to save documentation in Joggr &#x26; GitHub.</p></td></tr></tbody></table>

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

<table class="dashdraft-table"><tbody><tr class="dashdraft-table-row"><th class="dashdraft-table-header" colspan="1" rowspan="1"><p class="dashdraft-paragraph">Category</p></th><th class="dashdraft-table-header" colspan="1" rowspan="1"><p class="dashdraft-paragraph">Description</p></th></tr><tr class="dashdraft-table-row"><td class="dashdraft-table-cell" colspan="1" rowspan="1"><p class="dashdraft-paragraph">Request for Comment (RFC)</p></td><td class="dashdraft-table-cell" colspan="1" rowspan="1"><p class="dashdraft-paragraph">RFCs help developers think through a design or feature before coding. Use RFCs to think through a design &#x26; get feedback from the team.</p></td></tr><tr class="dashdraft-table-row"><td class="dashdraft-table-cell" colspan="1" rowspan="1"><p class="dashdraft-paragraph">Architecture</p></td><td class="dashdraft-table-cell" colspan="1" rowspan="1"><p class="dashdraft-paragraph">An architecture document shows the architecture of the system &#x26; how different components interact.</p></td></tr><tr class="dashdraft-table-row"><td class="dashdraft-table-cell" colspan="1" rowspan="1"><p class="dashdraft-paragraph">Guides</p></td><td class="dashdraft-table-cell" colspan="1" rowspan="1"><p class="dashdraft-paragraph">A guide shows developers how to complete a task (e.g. how to deploy).</p></td></tr><tr class="dashdraft-table-row"><td class="dashdraft-table-cell" colspan="1" rowspan="1"><p class="dashdraft-paragraph">Walkthroughs</p></td><td class="dashdraft-table-cell" colspan="1" rowspan="1"><p class="dashdraft-paragraph">A walkthrough shows developers how something works, often "walking" a developer through the code (i.e. How Authentication Works).</p></td></tr></tbody></table>

### Joggr Directory Structure

Below is our Directory Structure in Joggr. Please make sure to save all documents to the correct position.

<table class="dashdraft-table"><tbody><tr class="dashdraft-table-row"><th class="dashdraft-table-header" colspan="1" rowspan="1"><p class="dashdraft-paragraph">Folder</p></th><th class="dashdraft-table-header" colspan="1" rowspan="1"><p class="dashdraft-paragraph">Description</p></th></tr><tr class="dashdraft-table-row"><td class="dashdraft-table-cell" colspan="1" rowspan="1"><p class="dashdraft-paragraph"><code class="dashdraft-code-inline">Overview</code></p></td><td class="dashdraft-table-cell" colspan="1" rowspan="1"><p class="dashdraft-paragraph">Describe in 1-2 sentences what documentation should be saved to this folder.</p></td></tr><tr class="dashdraft-table-row"><td class="dashdraft-table-cell" colspan="1" rowspan="1"><p class="dashdraft-paragraph"><code class="dashdraft-code-inline">Standards</code></p></td><td class="dashdraft-table-cell" colspan="1" rowspan="1"><p class="dashdraft-paragraph">Describe in 1-2 sentences what documentation should be saved to this folder.</p></td></tr><tr class="dashdraft-table-row"><td class="dashdraft-table-cell" colspan="1" rowspan="1"><p class="dashdraft-paragraph"><code class="dashdraft-code-inline">Architecture</code></p></td><td class="dashdraft-table-cell" colspan="1" rowspan="1"><p class="dashdraft-paragraph">Describe in 1-2 sentences what documentation should be saved to this folder.</p></td></tr><tr class="dashdraft-table-row"><td class="dashdraft-table-cell" colspan="1" rowspan="1"><p class="dashdraft-paragraph"><code class="dashdraft-code-inline">Frontend</code></p></td><td class="dashdraft-table-cell" colspan="1" rowspan="1"><p class="dashdraft-paragraph">Describe in 1-2 sentences what documentation should be saved to this folder.</p></td></tr><tr class="dashdraft-table-row"><td class="dashdraft-table-cell" colspan="1" rowspan="1"><p class="dashdraft-paragraph"><code class="dashdraft-code-inline">Backend</code></p></td><td class="dashdraft-table-cell" colspan="1" rowspan="1"><p class="dashdraft-paragraph">Describe in 1-2 sentences what documentation should be saved to this folder.</p></td></tr></tbody></table>

### GitHub Directory Structure

Below is our approach to storing docs in GitHub. We have two places to store docs in GitHub:

<table class="dashdraft-table"><tbody><tr class="dashdraft-table-row"><th class="dashdraft-table-header" colspan="1" rowspan="1"><p class="dashdraft-paragraph">Area</p></th><th class="dashdraft-table-header" colspan="1" rowspan="1"><p class="dashdraft-paragraph">Description</p></th></tr><tr class="dashdraft-table-row"><td class="dashdraft-table-cell" colspan="1" rowspan="1"><p class="dashdraft-paragraph"><a target="_blank" rel="noopener noreferrer" class="dashdraft-link" href="github.com">Tech-Docs Repository</a></p></td><td class="dashdraft-table-cell" colspan="1" rowspan="1"><p class="dashdraft-paragraph">This repository holds documentation that does not make sense to put in a specific repository (i.e. Code Review Standards).</p></td></tr><tr class="dashdraft-table-row"><td class="dashdraft-table-cell" colspan="1" rowspan="1"><p class="dashdraft-paragraph"><code class="dashdraft-code-inline">/docs</code> directory in a code repositories</p></td><td class="dashdraft-table-cell" colspan="1" rowspan="1"><p class="dashdraft-paragraph">In every repository, we should have a <code class="dashdraft-code-inline">/docs</code> directory. If you are documenting something where it's obvious it should be saved in that repository, save it to the <code class="dashdraft-code-inline">/docs</code> folder.</p></td></tr></tbody></table>

> \[!NOTE]
>
> The Tech Docs Repostitory's file tree **should** mirror our Joggr file tree.

### When to Create JoggrDocs

We expect that software developers create documentation based on the following:

<table class="dashdraft-table"><tbody><tr class="dashdraft-table-row"><th class="dashdraft-table-header" colspan="1" rowspan="1"><p class="dashdraft-paragraph">RFC</p></th><th class="dashdraft-table-header" colspan="1" rowspan="1"><p class="dashdraft-paragraph">Arch.</p></th><th class="dashdraft-table-header" colspan="1" rowspan="1"><p class="dashdraft-paragraph">Guides</p></th><th class="dashdraft-table-header" colspan="1" rowspan="1"><p class="dashdraft-paragraph">Walkthroughs</p></th></tr><tr class="dashdraft-table-row"><td class="dashdraft-table-cell" colspan="1" rowspan="1"><p class="dashdraft-paragraph"><strong class="dashdraft-bold">MUST</strong> be created after approving the PRD and before starting development.</p></td><td class="dashdraft-table-cell" colspan="1" rowspan="1"><p class="dashdraft-paragraph"><strong class="dashdraft-bold">MUST</strong> create an architecture diagram for any new large project.</p></td><td class="dashdraft-table-cell" colspan="1" rowspan="1"><p class="dashdraft-paragraph"><strong class="dashdraft-bold">MUST</strong> be created or updated when a new standard process is introduced or an existing one is updated.</p></td><td class="dashdraft-table-cell" colspan="1" rowspan="1"><p class="dashdraft-paragraph"><strong class="dashdraft-bold">MUST</strong> be created when the team starts asking lots of questions about a certain part of our codebase (e.g. how does authentication work)</p></td></tr></tbody></table>

### How to Create JoggrDocs

We expect software developers to follow these standards when creating documentation.

<table class="dashdraft-table"><tbody><tr class="dashdraft-table-row"><th class="dashdraft-table-header" colspan="1" rowspan="1"><p class="dashdraft-paragraph">RFC</p></th><th class="dashdraft-table-header" colspan="1" rowspan="1"><p class="dashdraft-paragraph">Arch.</p></th><th class="dashdraft-table-header" colspan="1" rowspan="1"><p class="dashdraft-paragraph">Guides</p></th><th class="dashdraft-table-header" colspan="1" rowspan="1"><p class="dashdraft-paragraph">Walkthroughs</p></th></tr><tr class="dashdraft-table-row"><td class="dashdraft-table-cell" colspan="1" rowspan="1"><p class="dashdraft-paragraph"><strong class="dashdraft-bold">MUST</strong> use the RFC Template</p></td><td class="dashdraft-table-cell" colspan="1" rowspan="1"><p class="dashdraft-paragraph"><strong class="dashdraft-bold">MUST </strong>include a diagram</p></td><td class="dashdraft-table-cell" colspan="1" rowspan="1"><p class="dashdraft-paragraph"><strong class="dashdraft-bold">MUST</strong> use the How-To Guide template</p></td><td class="dashdraft-table-cell" colspan="1" rowspan="1"><p class="dashdraft-paragraph"><strong class="dashdraft-bold">MUST </strong>reference code examples where possible.</p></td></tr></tbody></table>
