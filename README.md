dynCrmDropZone
==============

DropzoneJS is a javascript library for allow file upload using drag-and-drop as well as multiple file selection (the more traditional way). For sending an email in Dynamics CRM 2011/2013 you are required to click 4-5 times per attachment and multiple attachment in the same click operation is not possible. However, CRM offers an OData endpoint for uploading attachments and this example code (*not yet production ready code*) uses that to allow drag-and-drop and multiple file uploads directly in the email form in a supported manner. 

These files were created in a few hours to prove the possibility. They are not yet production ready in quality.

**Package consists of three files:**
 * An HTML-file (the code that connects dropzoneJS and CRM)
 * A JS-file (unaltered library from dropzoneJS, just renamed to be CRM web resource friendly)
 * A CSS-file (unaltered default styling from dropzoneJS)

**Planned improvements:**
 * Use dropzoneJS optionally from a CDN instead of using it as web resources
 * Hide or show help when email is not yet saved (does not have ID yet, upload not possible before saving)
 * Custom styling to suit Dynamics CRM
 * Production worthy code
 * Test with more attachments

**How-to Install and Configure:**
 * Upload the three files as web resources in CRM
 * On the email form, insert web resource and point to the HTML file
 * Renaming the files is no issue, just remember to change the script and link element references in the top of the HTML

**Usage:**
 * Create a new email, save it
 * Click the upload filed to open file selection dialog, or drag in files to the browser window and this field
 * The attachment upload will begin
 * The attachment grid (standard component) will refresh for each uploaded attachment
 * Tested with PNG, JPG, XLSX, DOCX, PDF, PPTX, TXT.

**Screenshots:**

![File selection](/screenshots/scr0.png?raw=true "File selection")
![Uploading](/screenshots/scr1.png?raw=true "Uploading")
