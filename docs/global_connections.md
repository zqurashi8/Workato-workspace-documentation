# Global Connections

Workato provides **preconfigured global connections** managed in the HQ workspace. These **shared integrations** allow departments to access commonly used services **without needing to configure separate connections** for each workspace.

Using **global connections** ensures:
- **Security & Compliance** – API credentials are centrally managed.
- **Standardization** – Consistent integration settings across departments.
- **Reduced Duplication** – Avoids multiple redundant connections.
- **Faster Deployment** – No need to manually configure common integrations.

---

## Overview

Global connections are **centrally maintained** in the HQ workspace and are **automatically available** in new Workato workspaces. This eliminates the need for each department to create its own API connections, reducing **credential sprawl** and improving **security**.

By leveraging shared connections, teams can **focus on automating workflows** instead of managing authentication and integration details.

**Example Screenshot: Workato Global Connections Dashboard**
<p align="center">
  <img src="images/workato-global-connections.png" width="600"/>
</p>

---

## Available Global Connections

The following **pre-configured global connections** are available in Workato:

| **Service**                    | **Description** |
|--------------------------------|----------------|
| **Azure Active Directory**      | Used for identity and access management, allowing seamless authentication. |
| **Datadog**                     | Provides real-time application monitoring and analytics. |
| **Microsoft LogAnalytics API**  | Enables advanced log management and analysis for troubleshooting. |
| **Proofpoint**                  | Email security and threat protection platform. |
| **Autonomous Ops**              | Helps automate IT operations with AI-driven insights. |

These integrations ensure that **all Workato workspaces** can connect to **critical enterprise services** **without additional setup**.

---

## How to Use Global Connections

Since global connections are **centrally managed**, users **do not need to create new API connections** for these services.

### **Steps to Use a Global Connection**
1. **Open your Workato workspace**.
2. **Navigate to** `Connections`.
3. **Search for the required service** (e.g., `Azure Active Directory - Global`).
4. **Select the connection** and click **Use**.
5. **Verify that the connection is properly configured**.
6. **Start building recipes** using the shared connection.

**Example Screenshot: Selecting a Global Connection**
<p align="center">
  <img src="images/select-global-connection.png" width="600"/>
</p>

??? note "Automatic Access"
    These connections are **automatically available** to all new workspaces and do not require manual setup.

---

## Best Practices for Using Global Connections

To **ensure security and maintainability**, follow these best practices when using global connections:

### **1️⃣ Do Not Modify Global Connection Credentials**
- Global connections **are managed by HQ**.
- If an issue arises, **contact the Workato admin team** instead of modifying credentials.

### **2️⃣ Always Use Global Connections When Available**
- **Do not create duplicate API connections** in individual workspaces.
- If a required integration **is not available**, **submit a request** to the automation team.

### **3️⃣ Monitor Connection Usage**
- **Regularly check logs** for API call limits and failures.
- Use **Datadog or Microsoft LogAnalytics** to **track connection performance**.

---

## Common Issues & Troubleshooting

| **Issue** | **Possible Cause** | **Solution** |
|-----------|--------------------|--------------|
| **Connection is not visible** | Workspace is not correctly linked to HQ | Contact IT to verify workspace configurations. |
| **Authentication errors** | Expired credentials in HQ | Report the issue to the Workato admin team. |
| **API request limits exceeded** | Too many automations using the connection | Optimize recipe execution frequency. |

---

## ✅ Final Verification

To ensure proper usage of global connections:
1. **Verify that all recipes use global connections instead of personal API credentials**.
2. **Test a sample workflow** using the connection to confirm it functions correctly.
3. **Check Workato logs** to ensure proper authentication and integration.

By **leveraging shared global connections**, Workato workspaces **remain secure, scalable, and standardized** across the organization.

For further assistance, contact the **Workato automation team** or refer to the **Global Connections Documentation**.
