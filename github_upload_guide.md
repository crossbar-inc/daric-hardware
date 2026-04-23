# Guide: Uploading Files to the `daric-hardware` Repository via GitHub Web UI

This guide explains how to upload files to a specific directory in the **daric-hardware** repository **without using any git commands**. You only need a web browser.

---

## Prerequisites

- A GitHub account with admin access to the `crossbar-inc/daric-hardware` repository
- Files or folders ready on your local computer

---

## Repository Structure Overview

```
daric-hardware/
├── chip/
│   └── Daric-EVB-NTO/
├── reference_design/
│   ├── PHSM6/
│   │   ├── Assembly Drawing/
│   │   ├── BOM/
│   │   └── SCH/
│   ├── PHSM8/
│   │   ├── Assembly Drawing/
│   │   ├── BOM/
│   │   └── SCH/
│   └── PHSM8-EVB/
│       ├── Assembly Drawing/
│       ├── BOM/
│       └── SCH/
├── LICENSE
└── README.md
```

---

## Step 1: Navigate to the Target Directory

> [!IMPORTANT]
> You **must** navigate to the correct directory **before** uploading. Files will be placed in whatever directory you are currently viewing.

1. Open the repository page: `https://github.com/crossbar-inc/daric-hardware`
2. Click through the folder names to enter your target directory.

### Example

If you need to upload schematic files to `reference_design/PHSM8/SCH/`:

1. On the repository home page, click the **`reference_design`** folder.
2. Then click the **`PHSM8`** folder.
3. Then click the **`SCH`** folder.
4. Confirm the **breadcrumb path** at the top of the page reads:

```
daric-hardware / reference_design / PHSM8 / SCH /
```

Similarly, if you need to upload files to `chip/Daric-EVB-NTO/`:

1. Click the **`chip`** folder.
2. Then click the **`Daric-EVB-NTO`** folder.
3. Confirm the breadcrumb reads:

```
daric-hardware / chip / Daric-EVB-NTO /
```

> [!WARNING]
> If you see only `daric-hardware /` in the breadcrumb, you are at the **repository root** — not inside any subdirectory. Do **not** upload from here unless you intend to place files at the top level.

---

## Step 2: Start the Upload

1. Click the **Add file** button (near the top-right of the file list).
2. Select **Upload files** from the dropdown menu.

You will see a drag-and-drop area with the message *"Drag files here to add them to your repository"*.

---

## Step 3: Add Your Files or Folders

You have two options:

### Option A — Upload Individual Files

- Click **"choose your files"** (the link inside the drag-and-drop area), then select one or more files from your computer.
- Or simply **drag and drop** files from your file explorer into the upload area.

### Option B — Upload an Entire Folder

- **Drag and drop** an entire folder from your file explorer into the upload area.
- GitHub will preserve the folder structure automatically.

> [!TIP]
> You can upload **both files and folders at the same time** by selecting multiple items and dragging them all into the upload area.

> [!CAUTION]
> GitHub's web upload has a **file size limit of 25 MB per file**. If any individual file exceeds this limit, please contact the repository maintainer for assistance.

---

## Step 4: Commit Your Changes

1. Wait for all files to finish uploading (you will see a list of uploaded filenames).
2. In the **"Commit changes"** section at the bottom of the page:
   - Enter a short, descriptive **commit message** (e.g., `Upload PHSM8 schematic rev2.1`).
   - Leave the option set to **"Commit directly to the `main` branch"**.
3. Click the green **Commit changes** button.

---

## Quick Reference Checklist

| Step | Action |
|------|--------|
| 1 | Navigate into the **correct directory** (e.g., `reference_design/PHSM6/BOM/`) |
| 2 | Click **Add file** → **Upload files** |
| 3 | Drag & drop (or browse to select) your **files or folders** |
| 4 | Write a **commit message** and click **Commit changes** |

---

## Common Mistakes to Avoid

| ❌ Don't | ✅ Do |
|----------|-------|
| Upload from the repository root when files belong in a subdirectory | Always check the **breadcrumb path** before uploading |
| Leave the commit message empty or use vague text like "update" | Write a clear message, e.g., `Add PHSM8-EVB assembly drawing v3` |
| Upload files larger than 25 MB via the web UI | Contact the repository maintainer for large files |

---

## Need Help?

If you encounter any issues or need a new directory created, please reach out to the repository maintainer.
