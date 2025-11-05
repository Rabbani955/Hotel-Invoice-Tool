Modern HTML/CSS Invoice Generator (Single-File App)

This project is a clean, fully functional, and print-optimized invoice generator built as a single, self-contained HTML file. It allows users to quickly input key company, customer, and line item details, calculates Sub-Total, SGST, CGST, and Grand Total in real-time, and formats the result for a professional printout.

✨ Key Features

Real-Time Calculations: Automatically calculates item amounts, tax amounts (based on configurable SGST/CGST rates), and the final Grand Total as the user types.

Indian Tax System Support: Includes dedicated fields and calculation logic for SGST and CGST.

Total in Words: Automatically converts the final Grand Total amount into text (e.g., "ONE THOUSAND TWENTY RUPEES ONLY").

Dynamic Line Items: Users can add and delete multiple service/product line items on the fly.

Print Optimization: Uses dedicated CSS print styles (@media print) to hide the input form and optimize the invoice preview for a clean, professional paper printout.

Modern Design: Features a professional, high-contrast visual theme (dark headers, mango-gold highlights) with a responsive layout.

Single-File Deployment: All HTML, CSS, and JavaScript are contained within a single invoice-generator.html file, making it extremely easy to host, share, or embed.

🛠️ Technology Stack

HTML5: Structure and content.

CSS3 (Vanilla): Custom styling for the interface and specialized print media queries.

JavaScript (Vanilla): Core logic for data input, real-time calculations, dynamic row manipulation, and converting numbers to words.

🖨️ How the Print Function Works

The core requirement for this application was to produce a clean, ready-to-print document without showing the input controls.

The application achieves this through the window.print() method combined with CSS Media Queries:

JavaScript Trigger: When the "Print Invoice" button is clicked, the script executes window.print().

CSS Print Media Query: A dedicated style block (@media print) is activated by the browser during the print process.

Hiding Controls: This media query sets the input form element (.controls) to display: none;, ensuring only the generated invoice is visible to the printer.

Optimized Layout: The print styles also remove shadows, reset page margins, and use color-adjust: exact to ensure important colored headers (like the GST bar and detail headers) print correctly.
