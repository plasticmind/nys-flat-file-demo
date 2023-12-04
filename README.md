# NYS / Unav Alerts / Flat File Demo

## Description

This is a simple example of how a flat file system could serve a universal nav to New York State government sites, while still allowing content like alerts to be pulled in dynamically from a standalone file that is easy to edit.

The concept is straightforward:

- The content of the Universal Nav is pulled in from a flat file, instead of dynamically rendered from a CMS. This significantly reduces the overhead required to serve those requests and makes it easier to scale and maintain.
- The content of the alert is fetched from another file in the repository. If an alert exists, it gets rendered within the Universal Nav.
- Editorial teams responsible for managing the alert content would navigate to the alert file in GitHub, click the "Edit" button, and modify the contents of the file.
- Once the change is made, the editor would click "Commit changes" and add a brief description of the changes made (which can help track changes over time).
- The updated alert would be updated displayed on all NYS government websites using this embedded Universal Navigation. (There may be a short delay.)

Additional best practices would be requiring an additional review by engineering teams or a pull request to approve the change. This prevents any inadvertant mistakes from causing problems when the alerts deploy, without significant overhead.

## Demo

- Simple Dynamic Alert: https://plasticmind.github.io/nys-flat-file-demo/
- Structured Dynamic Alert: https://plasticmind.github.io/nys-flat-file-demo/structured.html
