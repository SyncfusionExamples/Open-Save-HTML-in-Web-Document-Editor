# Open-Save-HTML-in-Web-Document-Editor

This repository contains demo illustrates importing the HTML document and exporting the document of Syncfusion Word Processor (Document editor) component as HTML.

## Importing the HTML content

**Import HTML File:** "Import Html File" button allows you to import the html file in Files folder.

**Import HTML String:** "Import Html String" button allows you to import the html string which is given in text area. Here, we have used `LoadString()` API in controller file for conversion of HTML to SFDT. Then, loaded that SFDT in Document editor using `open()` method. You can also use `paste()` API to insert it in current position.

Please check this [`link`](https://ej2.syncfusion.com/documentation/document-editor/how-to/insert-text-in-current-position/#insert-the-rich-text-content) to know more about paste() API.

## Exporting the HTML content

In titlebar, `Download->HTML(html)` allows you to download the document as HTML format. 
* Here, we have converted the Document as SFDT format using `serialize()` API.
* Send that SFDT to backend and converted it to HTML using [`Save()`](https://ej2.syncfusion.com/documentation/document-editor/web-services/core/#save-as-other-file-formats-by-passing-sfdt-string) method.