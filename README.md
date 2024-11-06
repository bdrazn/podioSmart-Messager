This is a custom-built texting application for Podio, integrating with the **smrtphone.io** API to enable seamless SMS communication with leads and contacts. The app is designed to support lead conversion campaigns by automating outbound and inbound messaging, keeping track of communication, and improving response rates.

## Features

- **Automated Outbound Messaging**: Send scheduled SMS messages to contacts from Podio.
- **Real-Time Inbound Message Handling**: Capture responses from contacts directly in Podio.
- **Integration with smrtphone.io API**: Secure and reliable messaging through smrtphone.io.
- **Message History Tracking**: Record sent and received messages for each contact.
- **GlobiFlow Automation**: Custom workflows for follow-up messages, reminders, and lead recycling based on response status.

## Requirements

- **Podio Account**: Required to host the app and manage leads.
- **smrtphone.io API**: For SMS integration; you will need an API key and credentials.
- **GlobiFlow**: For automation workflows, message scheduling, and lead recycling.
- **Podio Permissions**: Ensure you have the necessary permissions to add apps and manage workflows in Podio.

## Installation

1. **Clone the Repository**: 
   ```bash
   git clone https://github.com/yourusername/podio-texting-app.git
   cd podio-texting-app
   ```

2. **Setup smrtphone.io API**: 
   - Go to [smrtphone.io](https://smrtphone.io) and generate an API key.
   - Add your API key to the configuration file in the app (e.g., `config.json`).

3. **Podio App Configuration**:
   - Create a Podio app to manage your contacts and leads.
   - Add custom fields as required for name, phone number, message status, etc.

4. **GlobiFlow Setup**:
   - Create flows in GlobiFlow to automate sending messages and handling responses.
   - Set up workflows based on your campaign requirements (e.g., follow-ups, reminders, lead recycling).

5. **Deploy**: Upload the application to your server or desired platform if running externally. Ensure server compatibility and necessary permissions for API calls.

## Usage

1. **Sending Messages**:
   - Add or import contacts into Podio.
   - Trigger workflows in GlobiFlow to send messages using the smrtphone.io API.
   - Messages will be logged under each contact’s profile for tracking.

2. **Receiving Messages**:
   - Configure inbound message handling to log responses directly in Podio.
   - Set GlobiFlow conditions to update message status and trigger follow-up actions.

3. **Automated Follow-Ups**:
   - Customize GlobiFlow workflows to send follow-up messages at specific intervals.
   - Use date-based calculations to schedule messages or recycle leads.

4. **Message Status Updates**:
   - Track sent, received, and pending messages.
   - Use custom views in Podio to monitor leads based on response status.


## Troubleshooting

- **API Errors**: Ensure that your smrtphone.io API key is correct and active.
- **Podio Permissions**: Check that your Podio account has the necessary permissions to create and manage apps and workflows.
- **Message Delays**: Verify your GlobiFlow schedules and check for any Podio rate limits if messages are delayed.
