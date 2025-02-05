# **Deployment Guide**

## **Environments**

<table class="dashdraft-table">
  <tbody>
    <tr class="dashdraft-table-row">
      <th class="dashdraft-table-header" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">Environment</p>
      </th>
      <th class="dashdraft-table-header" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">Description</p>
      </th>
      <th class="dashdraft-table-header" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">URL</p>
      </th>
    </tr>
    <tr class="dashdraft-table-row">
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><strong class="dashdraft-bold">Staging</strong></p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">Pre-production testing environment.</p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">staging.example.com</p>
      </td>
    </tr>
    <tr class="dashdraft-table-row">
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><strong class="dashdraft-bold">Production</strong></p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">Live environment.</p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">production.example.com</p>
      </td>
    </tr>
    <tr class="dashdraft-table-row">
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph"><strong class="dashdraft-bold">Sandbox</strong></p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">Rarely used, but available for experimentation.</p>
      </td>
      <td class="dashdraft-table-cell" colspan="1" rowspan="1">
        <p class="dashdraft-paragraph">sandbox.example.com</p>
      </td>
    </tr>
  </tbody>
</table>

## **Deployment Steps (GitHub Actions)**

* Push changes to the repository to trigger **GitHub Actions**.

* The workflow runs tests, builds, and packages the application.

* If tests pass, the deployment is pushed to **staging**.

* After verification, an **approval step** is required for **production deployment**.

* **Tag the release** before deploying to production.

```mermaid
graph LR;
    A[📌 Code Commit] -->|🚀 GitHub Actions Triggered| B[🛠️ Run Tests];
    B -->|📦 Build & Package| C[🚀 Deploy to Staging];
    C -->|✅ Verification| D[🏷️ Tag Release & Approve Deployment];
    D -->|🚀 Deploy to Production| E[🎉 Success];
    D -->|❌ Failure| F[🔄 Rollback];
```

## **Rollback Plan**

* Identify the issue and confirm rollback necessity.

* Use **GitHub Actions rollback workflow** to revert to the previous stable release.

```mermaid
graph LR;
    A[🚨 Issue Detected] -->|🔍 Assess Impact| B[✅ Confirm Necessity];
    B -->|⚙️ Run Script| C[🔄 Trigger Rollback Workflow];
    C -->|🔬 Run Tests| D[✅ Validate Rollback];
    D -->|📝 Post-Mortem| E[📄 Document & Improve];
```
