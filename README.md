# Guide to Setting Up and Using the Barcode Scanner Web App

## Current Version: 1.0.0


## Introduction
Welcome to the Barcode Scanner Input Web Application! This application is designed to facilitate efficient barcode scanning and data processing. It's particularly useful for businesses and individuals looking to integrate barcode scanning into their workflows, with a special focus on integration via webhooks for platforms like Make.com.

## Detailed Features
1. **Barcode Scanning and Validation**: 
   - The application allows users to scan barcodes.
   - It features real-time validation of barcode formats, expecting patterns like `123456-789-012`.

2. **Webhook Integration for Data Transmission**: 
   - Scanned barcode data is sent to a specified webhook URL, enabling integration with various platforms, including Make.com.

3. **Local Data Caching**: 
   - The application intelligently caches barcode data in local storage when offline.
   - This data is automatically sent when an internet connection is restored.

4. **Responsive Web Design**: 
   - Optimized for seamless functioning on both desktop and mobile devices.

5. **Internet Connection Monitoring**: 
   - Regular checks and updates about the internet connection status.

6. **Wake Lock Feature**: 
   - Prevents the device screen from going to sleep while the app is active, ensuring continuous scanning without interruptions.

7. **User Feedback and Error Handling**: 
   - Provides immediate feedback on the status of data transmission, including success and error messages.

8. **Automatic Focus Management**: 
   - Keeps the focus on the barcode input field, enhancing the user experience for continuous scanning.

9. **Event Handling for Wake Lock**: 
   - Manages the wake lock based on visibility changes and before the page unloads, ensuring efficient power management.

10. **Efficient Barcode Handling**: 
   - Once a barcode is scanned and validated, it is immediately sent or cached, and the input field is cleared for the next scan.

## Setup Instructions
1. **Webhook URL Configuration**:
    - Create your own webhook URL through Make.com.
    - Replace `'PASTE YOUR WEBHOOK HERE'` with your unique webhook URL in the script.

2. **Webhook Security**:
    - Secure your webhook on Make.com using IP address restrictions.
    - Utilize CIDR notation for specifying IP ranges.
    - Follow Make.com's guidelines for securing webhooks.

## Customization and Configuration
- **Barcode Format**: Adjust the regular expression in the `isValidBarcode` function to suit your barcode format requirements.
- **Webhook URL**: Insert the webhook URL provided by Make.com or your chosen platform.
- **Local Storage**: Change the local storage key `'cachedBarcodes'` if necessary.
- **Status Message Display**: Modify the duration and style of status messages within the `handleInput` and `sendData` functions.

## Important Notes for Users
- **Browser Compatibility**: The application requires a modern browser that supports JavaScript, local storage, and the Wake Lock API.
- **Wake Lock API**: This feature might not be supported in all browsers. Verify that your browser supports it for uninterrupted scanning.
- **Security Practices**: Follow recommended security practices for webhook setup to protect your data.
- **Error Handling**: Familiarize yourself with the error messages to troubleshoot issues related to internet connectivity or webhook errors.

## Conclusion
This Barcode Scanner Input Web Application is an efficient tool for businesses and individuals looking to integrate barcode scanning into their operations. Its features, including webhook integration, local caching, responsive design, and the wake lock feature, make it a versatile and user-friendly solution. Follow the setup instructions carefully and customize the application as needed to fit your specific requirements.

Feel free to reach out for any further assistance or queries. Happy scanning!
