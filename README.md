MFA Setup Generator
===================

A clean, professional, and entirely client-side web tool designed for IT administrators and security teams. This application generates scannable PDF setup guides to help end-users configure Multi-Factor Authentication (MFA) on their mobile devices.

This tool simplifies the onboarding process for authenticator apps (like Microsoft Authenticator, Google Authenticator, or Authy) by providing a single-page PDF containing a personalized QR code and clear, side-by-side platform instructions.

✨ Key Features
--------------

*   **Professional PDF Output:** Generates a high-fidelity A4 guide with clean typography, balanced whitespace, and corporate-friendly styling.
    
*   **Dynamic QR Generation:** Instantly converts TOTP secret keys (Base32) into scannable otpauth:// URIs.
    
*   **Privacy-First Architecture:** 100% client-side processing. Sensitive secret keys and emails never leave the user's browser or touch a server.
    
*   **Cross-Platform Ready:** Features dedicated, side-by-side instruction sets for both iOS and Android devices.
    
*   **Modern UI/UX:** Built using Tailwind CSS for a sleek interface and Lucide Icons for clear visual cues.
    

🚀 How to Use
-------------

1.  **Edit:** Open index.html in any text editoe of your choice and edit {Your Company Here} to be your company name for the footer of the generated PDF.

2.  **Launch:** Open index.html in any modern web browser.
    
3.  **Input Details:** \* Enter the user's **Company**:**Email Address**. This is copied from the TOTP setup page.
    
    *   Enter the **TOTP Secret Key** provided by your identity provider (e.g., Microsoft 365, Google Workspace).
        
4.  **Generate:** Click the **Generate Setup Guide** button.
    
5.  **Distribute:** The browser will generate and download a PDF. You can now securely send this file to the end-user.
    

🛠️ Customization & Branding
----------------------------

The file is designed to be easily modified to fit your company's branding:

*   **Colors & Branding:** Search for the #pdf-template ID in the HTML. You can swap the Tailwind color classes (e.g., text-blue-600, border-blue-600) with your brand's specific hex codes or color palette.
    
*   **Text Instructions:** The step-by-step guides are located within instruction-step containers. You can modify these to match your specific corporate IT policies.
    
*   **Icons:** The tool uses the Lucide icon library. You can swap icons by changing the data-lucide attributes.
    

📦 Technical Dependencies
-------------------------

This project leverages the following libraries via CDN:

*   [Tailwind CSS](https://tailwindcss.com/) - Utility-first CSS framework for the UI.
    
*   [QRCode.js](http://davidshimjs.github.io/qrcodejs/) - Logic for generating the scannable QR images.
    
*   [html2canvas](https://html2canvas.hertzen.com/) - Used to capture the HTML template as a high-resolution image.
    
*   [jsPDF](https://github.com/parallax/jsPDF) - Orchestrates the final PDF document creation.
    
*   [Lucide](https://lucide.dev/) - Beautifully simple community-run icon set.
    

📜 License
----------

This project is open-source and available under the [MIT License](https://opensource.org/licenses/MIT). Feel free to fork, modify, and distribute.

_Created with security and simplicity in mind._