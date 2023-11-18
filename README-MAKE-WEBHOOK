## User Guide: Creating a Secure Automated Workflow on Make.com

### Overview:
This guide will help you to create a secure, automated workflow in Make.com. The workflow starts with a secured webhook and includes steps like adding a delay, checking conditions, using Boomerangme to update a card, and ignoring certain conditions.

### Prerequisites:
- A Make.com account.
- A basic understanding of webhooks, IP restrictions, and the Boomerangme application.
- Access to the services you plan to integrate.

### Instructions:

#### 1. Securely Setting Up a Custom Webhook:
   - Log into your Make.com account and navigate to the **Webhooks** service.
   - Choose to create a new **Custom Webhook**.
   - During the setup, you will see an option for IP restrictions. Enter a whitelist of IP addresses that are authorized to trigger this webhook. Input the addresses separated by commas.
     - To whitelist a range of IP addresses, use CIDR notation (e.g., `192.168.1.0/24`).
     - Leave this field blank if you do not wish to impose any restrictions, but this is not recommended for security purposes.
   - Save the webhook configuration and note the URL provided for triggering this scenario.

#### 2. Adding a Delay:
   - Insert a **Delay** module into your workflow.
   - Configure the delay duration as needed for your process.

Adding a delay in Make.com helps manage the timing of automated actions, prevent API rate limit issues, and coordinate sequential task execution.

#### 3. Condition Check:
   - Place a condition check in the workflow to ensure that the process continues only if certain criteria are met.

#### 4. Using Boomerangme:
   - Add the **Boomerangme** module.
   - Authorize Boomerangme to interact with the application and select the specific action to be performed on the card.

#### 5. Setting up Ignore Action:
   - Finally, implement an **Ignore** module to define any actions or conditions that should be skipped or halted in the workflow.

#### 6. Testing Your Scenario:
   - Perform a test by sending a request to your webhook URL from an allowed IP address.
   - Check that each step of the scenario executes correctly, adjusting settings if necessary.

#### 7. Activating Your Scenario:
   - Once testing is successful, activate your scenario to have it run automatically in response to future webhook triggers.

### Security Note:
Ensure that you maintain a current list of authorized IP addresses and update the whitelist as needed to prevent unauthorized access.

### Final Steps:
- Document the scenario setup and usage instructions, including the secure webhook URL and IP restrictions, to share with your team or end-users.
- Regularly review and update your IP restrictions to maintain security and ensure uninterrupted workflow operation.

