---
title: "Notion"
slug: /app-integrations/notion/
---

Notion is an all-in-one workspace platform for notes, documents, wikis, and project management. Integrating Notion into appse ai enables you to automate page creation, database management, content updates, and more — directly within your workflows.

---

## Set Up Credential

:::info

Before you create a credential for Notion using appse ai, ensure you have a Notion account and have set up an Internal Integration from the Notion integrations portal to obtain an Integration Token.

:::

### Required Fields

You'll be asked to fill in the following details:

| Field              | Description                                                  |
| ------------------ | ------------------------------------------------------------ |
| Connection Name    | A name to help you identify this connection                  |
| Integration Token  | The Internal Integration Token from your Notion integration  |

---

### Step-by-Step Guide

#### 1. Open the Credential Form

Click **Select a Credential** and choose **Notion** from the application list. Add your **Connection Name**.
<img src="/img/credentials/notion/create-new-cread.png" alt="appse ai Claude Select Credential" width="700"/>

#### 2. Go to Notion Integrations

Navigate to [https://www.notion.so/profile/integrations](https://www.notion.so/profile/integrations) and click **"New integration"**.

#### 3. Set Integration Type to Internal

Under integration type, select **"Internal"**.
Click on Create a new integration

:::info

Select **Internal** to get an Integration Token. Internal integrations provide a bearer token that can be used directly to authenticate API requests.

:::

<img src="/img/credentials/notion/create-new-cred-notion.png" alt="appse ai Claude Select Credential" width="700"/>

#### 4. Fill in Integration Details

Fill in the following:

- **Name**: Give your integration a recognisable name.
- **Associated Workspace**: Select the Notion workspace you want this integration to access.

Click **"Create"** once done.

<img src="/img/credentials/notion/click-save-cred-notion.png" alt="appse ai Claude Select Credential" width="700"/>

<img src="/img/credentials/notion/configure-cred-notion.png" alt="appse ai Claude Select Credential" width="700"/>

#### 5. Copy Your Integration Token

After saving, copy the **Internal Integration Token** (also referred to as the Secret) from the integration page.

<img src="/img/credentials/notion/copy-integration-key.png" alt="appse ai Claude Select Credential" width="700"/>

#### 6. Paste the Token in appse ai

Return to the appse ai credential form. Paste the **Integration Token** into the respective field and click **"Save"** to store and validate your credential.

<img src="/img/credentials/notion/enter-your-integration-token.png" alt="appse ai Claude Select Credential" width="700"/>

<img src="/img/credentials/notion/Create-credential-notion-appseai.png" alt="appse ai Claude Select Credential" width="700"/>

:::warning

After connecting, make sure your Notion integration has access to the specific pages or databases you want to work with. In Notion, open the relevant page → click the **"..."** menu → go to **"Connections"** → add your integration.

:::

---

## Triggers and Actions

Here is a list of the available triggers and actions for Notion:

### Triggers

- **On Page Added to Database** — Fires whenever a new page is added to a specified Notion database. Use this trigger to start a workflow automatically when a new database entry is created.

- **On Page Updated in Database** — Fires whenever an existing page inside a specified Notion database is updated. Use this trigger to react to changes in database records in real time.

---

### Actions

- **Append Block** — Appends one or more new content blocks (such as paragraphs, headings, bullet points, code blocks, or callouts) to the end of an existing Notion page or block. Useful for adding content to a page without overwriting existing data.

- **Archive Page** — Archives a specified Notion page, removing it from active view without permanently deleting it. The page can be restored later from Notion's archive.

- **Create Page in Database** — Creates a new page inside a specified Notion database with the provided properties, content blocks, icon, cover, and optional template support. Use this to programmatically add new records or entries to a database.

- **Get Child Blocks By BlockId** — Retrieves all child blocks nested inside a specified Notion page or block. Use this to read the full content structure of a page.

- **Get Database by ID** — Fetches the metadata and schema of a specified Notion database, including its properties and column definitions.

- **Get Page by PageId** — Retrieves the properties and metadata of a specified Notion page by its ID. Use this to read the current state of a page before updating it.

- **Get User by ID** — Fetches the details of a specific Notion user by their user ID, including their name and email address.

- **Get Users** — Retrieves a list of all members in your Notion workspace. Useful for assigning tasks or filtering content by user.

- **Query Database** — Queries a Notion database with optional filters and sorting to retrieve matching pages. Use this to search for specific records within a database.



- **Update Page** — Updates the properties, icon, cover, or archive status of an existing Notion page. Use this to edit database record fields, change page titles, or update any other page-level properties.

---

## Support

Need help? Contact our support team at [hello@appse.ai](mailto:hello@appse.ai)