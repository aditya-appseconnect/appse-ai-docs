---
title: "Amazon Seller Central"
slug: /app-integrations/amazon-seller-central/
---

Amazon Seller Central is the marketplace for managing your Amazon selling account. It allows you to list products, manage inventory, fulfill orders, and track your business performance. Integrating Amazon Seller Central into appse ai enables you to automate order management, feed submissions, financial reporting, and more — directly within your AI-powered workflows.

---

## Set Up Credential

:::info

Before you create a credential for Amazon Seller Central using appse ai, ensure you have an Amazon Seller Central account and have registered as a developer (or authorized a developer app).

:::

---

### Step-by-Step Guide

#### 1. Open the Credential Form

Click **Select a Credential** and choose **Amazon Seller Central** from the application list.

<img src="/img/credentials/amazon-seller-central/Create-new-cread-appseai-amazon-seller-central.png" alt="appse ai Amazon Seller Central Connection Name" width="700"/>

This opens the Amazon Seller Central credential form. Add your **Connection Name**.


#### 2. Sign In to Amazon Seller Central

Go to [Amazon Seller Central](https://sellercentral.amazon.com) and sign in with your seller account.

#### 3.Access Your  Application

  Click the save and authorise button



<img src="/img/credentials/amazon-seller-central/seleect-region-seller-central.png" alt="appse ai Amazon SP-API Developer Apps" width="700"/>

#### 4. Authorize the App and Complete Two-Step Verification

Log in to your Amazon Seller Central account and complete the two-step verification process.
Follow the Login with Amazon (LWA) flow to authorize your application against your Seller account.

<img src="/img/credentials/amazon-seller-central/enter-password-seller-central.png" alt="appse ai Amazon Seller Central Refresh Token" width="700"/>


<img src="/img/credentials/amazon-seller-central/enter-otp-seller-central.png" alt="appse ai Amazon Seller Central Refresh Token" width="700"/>


 Once the verification is successfully completed, your credentials will be automatically validated and confirmed within appse ai — no additional configuration is required.
 

<img src="/img/credentials/amazon-seller-central/select-country-seller-central.png" alt="appse ai Amazon Seller Central Save Credential" width="700"/>



<img src="/img/credentials/amazon-seller-central/click-confirm-seller-central.png" alt="appse ai Amazon Seller Central Save Credential" width="700"/>




<br/>

:::warning

Keep your credentials secure.
:::

---

## Triggers and Actions

Here is a list of the available triggers and actions for Amazon Seller Central:

### Triggers

- **Feed Created or Updated** — Initiates the workflow when a feed is submitted or its processing status changes . This trigger is useful for monitoring the outcome of bulk data uploads in real time.

- **New Sales Order Financial Event** — Initiates the workflow when a new sales order financial event is recorded in your account, such as a charge, refund, or fee associated with a completed order.

- **New Return Financial Event** — Initiates the workflow when a return-related financial event is logged, such as a customer refund or return adjustment that impacts your account balance.

---

### Actions

- **Create Feed Document** — Creates a new feed document and returns a secure upload URL. This is the required first step before submitting a feed to Amazon. A **Content Type** for the feed data must be specified.

- **Create Feed** — Submits a feed to Amazon Seller Central for processing. This action is to be performed after uploading your data to the URL returned by the **Create Feed Document** action. Requires a **Feed Type** and the **Feed Document ID**.

- **Get Feed** — Retrieves the details and current processing status of a specific feed. Requires a **Feed ID** returned from the **Create Feed** action.

- **Get Order Items** — Retrieves the line items associated with a specific order, including product details, quantities, and pricing information. Requires an **Order ID**.

- **Get Order Buyer Info** — Retrieves buyer information associated with a specific order, such as the buyer's name and email address. Requires an **Order ID**.

- **Get Orders** — Retrieves a list of orders based on specified filters such as order status, marketplace, and date range. This action is useful for monitoring recent sales activity across your account.

- **Get Order Address** — Retrieves the shipping address associated with a specific order. Requires an **Order ID**. Please note that address data may be obfuscated for certain marketplace regions in accordance with Amazon's data protection policies.

- **Get Shipment Items** — Retrieves the items included in a specific inbound shipment to an Amazon fulfillment center. Requires a **Shipment ID**.

---

## Support

Need help? Contact our support team at [hello@appse.ai](mailto:hello@appse.ai)