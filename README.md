# HTML to PDF Wordpress Plugin

This WordPress plugin enables users to convert HTML/web pages into PDF documents while preserving layout, styling, and content. The plugin is built using the powerful **DOMPDF** library to handle the conversion process.

---

## Features

- Convert any URL to a PDF document.
- Preserve text, images, formatting, tables, lists, and hyperlinks.
- Choose paper size (e.g., A4, Letter) and orientation (Portrait or Landscape).
- Generate and download PDFs directly from the WordPress dashboard or frontend.
- User-friendly shortcode and admin menu integration.

---

## Installation Instructions

### 1. Clone or Download the Plugin

Clone or download this repository into your WordPress plugin directory:
```bash
git clone https://github.com/your-username/html-to-pdf-plugin.git
```
Or download the ZIP file, extract it, and upload the folder to `wp-content/plugins/`.

### 2. Install the DOMPDF Library

The plugin uses **DOMPDF** for the PDF generation process. Follow these steps to set up the library:

1. Download the DOMPDF library from its official repository:
   [https://github.com/dompdf/dompdf](https://github.com/dompdf/dompdf)

2. Extract the DOMPDF library and place its contents in the following directory inside the plugin folder:
   ```
   wp-content/plugins/html-to-pdf-plugin/lib/dompdf/
   ```

   The folder structure should look like this:
   ```
   html-to-pdf-plugin/
   ├── lib/
   │   └── dompdf/
   │       ├── autoload.inc.php
   │       ├── src/
   │       └── ...
   ├── assets/
   ├── html-to-pdf-plugin.php
   └── ...
   ```

3. Ensure the `autoload.inc.php` file is present in the `dompdf` directory.

### 3. Activate the Plugin

- Log in to your WordPress dashboard.
- Navigate to **Plugins > Installed Plugins**.
- Find the **HTML to PDF Converter** plugin and click **Activate**.

---

## Usage Instructions

### 1. Admin Dashboard

Once activated, a new menu item labeled **HTML to PDF** will appear in the WordPress admin sidebar:

1. Go to **HTML to PDF**.
2. Enter the desired URL in the provided input field.
3. Select the paper size and orientation.
4. Click the **Generate PDF** button to download the PDF to your computer.

### 2. Frontend Shortcode

You can also add a PDF generation form to any page or post using the following shortcode:
```plaintext
[html_to_pdf]
```

This will display a form where users can input a URL and customize the PDF options.

---

## Requirements

- WordPress 5.0 or higher
- PHP 7.2 or higher
- DOMPDF library installed in the correct directory

---

## Folder Structure

```
html-to-pdf-plugin/
├── lib/
│   └── dompdf/          # DOMPDF library
├── assets/
│   ├── css/             # Stylesheets for the plugin
│   └── js/              # JavaScript files
├── html-to-pdf-plugin.php # Main plugin file
├── README.md            # Readme file
└── ...
```

---

## Support

If you encounter issues while setting up or using the plugin, please create an issue in the [GitHub repository](https://github.com/your-username/html-to-pdf-plugin/issues).

---

## License

This plugin is licensed under the MIT License. See the LICENSE file for details.

---

## Screenshots

### Admin Dashboard
![Admin Dashboard Screenshot](link-to-admin-dashboard-screenshot)

### Frontend Form
![Frontend Form Screenshot](link-to-frontend-form-screenshot)

---

## Contributing

Contributions are welcome! Feel free to fork the repository and submit a pull request with your improvements.

