# Workspace Setup

This section provides a **step-by-step guide** on setting up a new Workato workspace. Following these guidelines ensures consistency, security, and efficiency across all departments.

Setting up a workspace properly helps:
- **Maintain standardization** across the organization.
- **Optimize automation performance** with proper task limits and concurrency settings.
- **Ensure security** by assigning appropriate roles and using best practices.

---

## Step 1: Create a New Workspace

To create a Workato workspace, follow these steps:

1. **Log in to Workato HQ Workspace** using an administrator account.
2. **Navigate to:**  
   - `Automation HQ` → `Create Workspace`.
3. **Fill in workspace details:**
   - **Workspace Name:** Use only the **Department Name** (e.g., `Finance`, `Security`, `HR`).
   - **Task Limit:** Default is `250,000` tasks. Increase in increments based on workload requirements.
   - **Additional Concurrency:** Default is `1`. Increase if high parallel execution is required.
   - **Active OPA Limit:** Default is `2` OPAs. Increase if integrating with on-premise systems.
4. **Assign a Workspace Moderator (MasterChef role).**
5. **Save and finalize workspace settings.**

**Example Screenshot: Workato Create Workspace Page**
<p align="center">
  <img src="images/workato-create-workspace.png" width="600"/>
</p>

---

## Step 2: Assign a Workspace Moderator

Each workspace requires a **Workspace Moderator**, responsible for governance, security, and troubleshooting.

### **Who Can Be a Moderator?**
- **MasterChefs** within the department are the primary candidates.
- Each department **may nominate another user** if necessary.

### **Responsibilities of a Workspace Moderator**
✅ Oversee **workspace governance & monitoring**.  
✅ Ensure **security policies are followed**.  
✅ Manage **workspace-level task limits and concurrency settings**.  
✅ Approve **automation deployments and workflow modifications**.

---

## Workspace Configuration Settings

| **Setting** | **Default Value** | **Purpose** | **Guidance** |
|------------|------------------|------------|-------------|
| **Workspace Name** | `{Department}` (e.g., `Finance`, `Security`, `TechOps`) | Standardized for easy identification | Avoid generic names like `IT`, use `TechOperations` instead |
| **Task Limit** | `250,000 tasks` | Prevents excessive resource consumption | Can be increased in `50K increments` if needed |
| **Additional Concurrency** | `1` | Controls how many recipes can run simultaneously | Increase if multiple workflows require parallel execution |
| **Active OPA Limit** | `2 OPAs` | Ensures redundancy for on-premise integrations | Increase for workspaces integrating with databases or local file systems |

---

## Workspace Best Practices

Following **best practices** ensures that your workspace is **optimized, secure, and scalable**.

### **1️⃣ Naming Conventions**
- **Always use the department name** for easy workspace identification.
- ❌ **Bad Example:** `IT_Automations`
- ✅ **Good Example:** `TechOperations`

### **2️⃣ Role-Based Access Control**
- **Use Entra ID (Azure AD) for role-based authentication.**
- Assign users to **SousChef, Chef, or MasterChef roles** based on training completion.

### **3️⃣ API & Service Account Policies**
- **Avoid personal API connections.** Always use service accounts for external integrations.
- If the workspace requires an API connection, **use a dedicated service account** instead of individual credentials.

### **4️⃣ Automation Best Practices**
- Use **prebuilt Workato templates** whenever possible to standardize automation workflows.
- **Review automation workflows** before deployment to prevent failures.
- **Monitor task execution logs** to identify inefficiencies and bottlenecks.

---

## Common Issues & Troubleshooting

| **Issue** | **Possible Cause** | **Solution** |
|-----------|--------------------|--------------|
| **Workspace not visible in dashboard** | User lacks permission | Verify role assignment in Workato and Entra ID. |
| **API connections failing** | Using personal credentials instead of a service account | Update connection settings to use a department-wide service account. |
| **Recipe execution limits exceeded** | Too many parallel workflows running | Optimize workflows and request an increased task limit if necessary. |

---

## ✅ Final Verification

Before **finalizing a new workspace**, perform the following **checks**:
1. **Ensure all users are assigned to appropriate Entra ID groups**.
2. **Verify API credentials use a service account** instead of personal login details.
3. **Test a sample workflow** to ensure recipe execution functions properly.
4. **Enable monitoring and alerting** to track automation performance.

Once these steps are complete, your **Workato workspace is fully configured and ready for automation deployment**.

For further assistance, contact the **Workato Automation Team**.
