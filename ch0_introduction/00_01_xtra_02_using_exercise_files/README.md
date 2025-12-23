# 00_01 Extra Content 02: Using Exercise Files From the Course

In this course, you’ll work with **lesson-specific repositories** that you create yourself. The recommended workflow is to download the course exercise files once, then upload the relevant files into a new repository for each lesson.

The steps below walk you through:

1. Downloading the exercise files
2. Creating a new repository
3. Uploading the lesson files while preserving their folder structure

![Image](https://s31.postimg.cc/r45t0i9a3/imageedit_9_4620369683.jpg)

![Image](https://docs.github.com/assets/cb-29762/images/help/repository/repo-create-global-nav-update.png)

![Image](https://saraford.net/wp-content/uploads/2016/12/image44.png)

---

## Prerequisites

* You’re signed in to your GitHub account.
* You have access to the course exercise files repository.

---

## Step 1: Download the exercise files as a ZIP

1. Navigate to the **exercise files repository** for the course.
2. Select the **Code** button.
3. Select **Download ZIP**.
4. Save the ZIP file to a location on your computer (for example, your *Downloads* folder).
5. Once the download completes, **expand/unzip** the file so you can view the contents on your local system.

> Tip: Make a note of where the files are extracted—you’ll need to access them again when uploading lesson files.

---

## Step 2: Identify the lesson files you need

1. Open the extracted exercise files folder.
2. Locate the directory for the lesson you’re currently working on
   (for example: *Chapter 1, Lesson 4 – Setup CI for Go*).
3. Review the contents of that lesson folder.

   * Many lessons include **multiple files and directories**
   * The folder structure is important and must be preserved when uploading

---

## Step 3: Create a new repository for the lesson

1. In GitHub, select **New repository**.
2. Enter a **repository name**.

   * Recommended: use the **lesson identifier or lesson name** to make it easy to find later
     (for example: `0104ci4go`)
3. Enter a short **description** (for example: *Exercise files for lesson 0104*).
4. Choose **Public** or **Private**, based on your preference.
5. Select **Add a README file**.
6. Select **Add .gitignore**.

   * Choose the language used in the lesson (for example, **Go**).
7. Do **not** add a license.
8. Select **Create repository**.

---

## Step 4: Upload the lesson files

1. In your new repository, select **Add file**.
2. Select **Upload files**.
3. Open your system’s file browser:

   * **Finder** on macOS
   * **File Explorer** on Windows
4. Navigate to the lesson folder you identified earlier.
5. **Ensure hidden files are visible** (files starting with a dot, such as `.gitignore`).

   * Some lessons include hidden files that are required.
6. Select **all files and folders** for the lesson.
7. Drag the selected files and folders **into the browser window**.

> Important: Drag-and-drop from your file browser is the best way to upload folders.
> Using the file picker to upload individual files does **not** preserve directory structure.

---

## Step 5: Commit the uploaded files

1. Wait while GitHub processes the files and folders.

   * GitHub will preserve the full directory structure.
2. Scroll to the bottom of the page.
3. Select **Commit changes**.

---

## Step 6: Verify the upload

1. Review the repository contents.
2. Confirm that:

   * Files display with **file icons**
   * Directories display with **folder icons**
3. Select a folder to verify that its subfolders and files are present.

If the structure matches the original lesson folder on your system, the upload was successful.

---

You can now repeat this process for each lesson in the course by creating a new repository and uploading the corresponding exercise files.

<!-- FooterStart -->
---
[← 00_01 Extra Content 01: Create a GitHub Organization for Your Course Repositories](../00_01_xtra_01_create_github_organization/README.md) | [00_02 Explore the Capabilities of Github actions →](../00_02_explore_the_capabilities_of_github_actions/README.md)
<!-- FooterEnd -->
