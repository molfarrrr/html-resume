# html-resume
A single-page résumé template done purely with HTML and CSS, which can be rendered into PDF through web browsers' print-to-PDF functionality, making a nice, sleek, professsional and ready-to-print résumé.

As the résumé is purely typeset with HTML and CSS, it's highly customizable (e.g. if you want an "objective" section, just copy-paste a few HTML elements) and does not require proprietary software. All you need is a text editor and a web browser (see compatibility section below). Oh, maybe some intermediate CSS knowledge. And, since it's open source with Apache License, you're allowed (and encouraged!) to create your own fine-tuned template and share with others.

# Compatibility and Known Issues/Limitations
* I have only tested this project on latest release version of Firefox (56 as of writing) and Google Chrome (61) on macOS 10.13 (High Sierra).
* It's my intention to support other browsers/platforms (like IE Edge on Windows?) as long as the browser sufficiently supports the required CSS features: ``calc()``, ``var()``, ``flexbox``, ...etc, and does not require (too many) dirty tricks. PRs or comments welcome!
* **No hyperlinking functionality in rendered PDF** as browers's print-to-PDF process is merely "flattening to digital paper".
* Other browser-specific hacks are as commented in the code.

# Paper Size/Orientation
* Currently letter portrait only. PRs welcome for other paper sizes --- especially A4!

# Actually Rendering the PDF
* Again...I've only tried on the said version of Firefox & Chrome, on macOS.
* Just open the HTML file with the browser. No need to serve the document from any kind of web server --- the ``file:///`` protocol should be good enough.
* On Firefox:
  * You probably need to remove any page margins in **about:config**.
  * Uncheck **Ignore Scaling and Shrink To Fit Page Width**.
  * Check **Print Background Colors**.
  * Clear out the headers and footers.
  * Save as PDF.
* On Google Chrome:
  * Set **Margin** to **None**.
  * Print **Background Graphics**.
  * Don't print headers and footers.
  * Save as PDF.
