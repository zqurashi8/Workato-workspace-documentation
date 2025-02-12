# Shared Templates

Workato provides **pre-built automation templates** that departments can use to streamline processes. These templates help teams **quickly implement common workflows** without needing to build recipes from scratch.

Using shared templates ensures:
- **Standardization across teams** – Automations follow best practices.
- **Faster deployment** – No need to start from zero.
- **Reduced errors** – Pre-configured logic helps prevent common mistakes.
- **Empowerment for citizen developers** – Non-technical users can implement automations easily.

---

## Overview

Shared templates allow teams to **accelerate automation adoption** while maintaining **security and consistency**. They provide **ready-to-use Workato recipes** that can be imported into any workspace and customized to fit specific departmental needs.

### **Key Benefits of Shared Templates**
✅ **Reduces time to implement** automations.  
✅ **Ensures compliance** with organizational policies.  
✅ **Encourages citizen development** by making automation more accessible.  
✅ **Prevents duplication of effort** – teams can leverage existing work.  

---

## Available Templates

Workato offers **a variety of automation templates** for different use cases.

=== "Available Templates"
    - **Slack Workbot Automation** – Automates alerts, approvals, and notifications.
    - **Employee Onboarding Workflow** – Automates account creation and access permissions.
    - **Finance Reconciliation Reports** – Syncs transaction data across financial systems.
    - **IT Ticketing System Integration** – Connects IT service requests with ticketing platforms.
    - **Customer Support Case Management** – Automates case handling between CRM and support teams.

**Example Screenshot: Workato Template Library**
<p align="center">
  <img src="images/workato-template-library.png" width="600"/>
</p>

These templates are **continuously updated** based on **feedback and new automation requirements**.

---

## How to Access

Templates are stored in a **central repository** and can be imported into any Workato workspace.

??? info "Steps to Import Templates"
    1. **Go to Box** and locate **Workato Pre-Built Templates**.
    2. **Download the template package**.
    3. **Import the template** into your Workato workspace.
    4. **Review and customize** the template based on your department’s needs.
    5. **Test and deploy** the automation.

### **Importing Templates into Workato**
To import a template:
1. **Navigate to**: `Recipes` → `Import Recipe`.
2. Select the **template file (.wrk) from Box**.
3. Choose the **target workspace**.
4. Review any **environment-specific variables** and update them as needed.
5. Save and **deploy the imported recipe**.

---

## Best Practices for Using Shared Templates

While templates **simplify automation**, teams should follow best practices to ensure **security and maintainability**.

### **1️⃣ Always Review Before Deployment**
- Ensure that the template **meets your department's needs**.
- Check for **required API connections** and **permissions**.
- Update **workspace-specific configurations**.

### **2️⃣ Use Environment Variables for Credentials**
- Avoid **hardcoding API keys or credentials**.
- Instead, use **Workato environment properties**.

### **3️⃣ Optimize and Customize as Needed**
- Modify templates to fit **specific business processes**.
- Remove **unnecessary steps** to improve performance.

---

## Troubleshooting & Common Issues

| **Issue** | **Possible Cause** | **Solution** |
|-----------|--------------------|--------------|
| **Template import fails** | File format is incorrect | Ensure you are using a `.wrk` file exported from Workato. |
| **Recipe does not work as expected** | Missing API connections | Verify that required connections are properly configured. |
| **Automation does not trigger** | Incorrect trigger configuration | Review the trigger event and test execution. |

---

## ✅ Final Verification

Before **fully deploying** an imported template:
1. **Run test executions** to validate the workflow.
2. **Ensure that necessary integrations** (Slack, ServiceNow, HR systems) are correctly configured.
3. **Document any modifications** to ensure consistency across workspaces.

By following these best practices, teams can **leverage shared templates effectively**, ensuring that automations are scalable, secure, and properly optimized.

For further assistance, reach out to the **Automation Team** or refer to the **Workato Shared Templates Library**.
