
# Converting DOCX to Markdown for Obsidian

## **User Prompt**
> I have a microsoft word document in docx format. It contains both text and images. I would like to convert this document to markdown format to store in Obsidian. Is there a way to convert a docx to markdown, saving the images in the word document as individual image files and linking to those image files in the markdown code?

## **Gemini Response**
Yes, you can definitely do this. The most reliable and powerful tool for this job is a command-line program called **Pandoc**.

For a user-friendly option directly within your vault, you can also use an **Obsidian community plugin**.

Here are the two best methods to convert your `.docx` file, extract the images, and correctly link them in Markdown.

---

### Method 1: Use Pandoc (Recommended)

Pandoc is a universal document converter and is the industry standard for this kind of task. It correctly extracts images from the Word file and places them in a new folder, automatically writing the Markdown links to point to those new files.

**Step 1: Install Pandoc**

If you don't already have it, you'll need to install it.
* **On Windows:** The easiest way is to download and run the installer from the [Pandoc website](https://pandoc.org/installing.html).
* **On macOS (using Homebrew):** If you use Homebrew, just open Terminal and run: `brew install pandoc`
* **On Linux (using apt):** `sudo apt-get install pandoc`

**Step 2: Run the Conversion Command**

1.  Open your command-line tool (Terminal, Command Prompt, or PowerShell).
2.  Navigate to the folder where your `.docx` file is located using the `cd` command (e.g., `cd "C:\My Documents"`).
3.  Run the following command, replacing `your-file.docx` with your file's name:

    ```bash
    pandoc "your-file.docx" --extract-media=./ -o "output-file.md"
    ```

**What this command does:**
* `"your-file.docx"`: The Word document you are converting.
* `--extract-media=./`: This is the key part. It tells Pandoc to extract all images and other media files. The `./` instructs it to create a **new folder named `media`** in your current directory.
* `-o "output-file.md"`: This specifies the name of the new Markdown file that will be created.

**Step 3: Move Files to Obsidian**

After running the command, you will have two new things in your folder:
1.  `output-file.md` (your new note)
2.  A folder named `media` (containing all your extracted images)

Simply **drag both the `.md` file and the `media` folder** into your Obsidian vault. The Markdown file will already contain the correct relative links (like `![](./media/image1.png)`), and everything will work perfectly.

---

### Method 2: Use an Obsidian Plugin

If you prefer to avoid the command line, you can perform the conversion directly inside Obsidian.

1.  In Obsidian, go to **Settings** > **Community plugins**.
2.  Turn off "Restricted mode" if it's on.
3.  Click **Browse** and search for a plugin called **"Docxer"**.
4.  **Install** and then **Enable** the plugin.
5.  Drag your `.docx` file directly into your Obsidian vault (just like you would an image or PDF).
6.  Find the `.docx` file in Obsidian's file explorer. When you click on it, instead of seeing a preview, you should see a button that says **"Convert"**.
7.  Clicking this button will convert the file to Markdown and handle the extraction of images for you.

This method is simpler as it keeps everything inside your vault, but Pandoc (Method 1) is generally more powerful and offers more control if you have complex documents.

For a visual guide on using Pandoc to convert file types, this video provides a good overview of its command-line-based operation.
[A quick look at Pandoc](https://www.youtube.com/watch?v=04GPPtuhjyI)

## **User Prompt**
> Say I use the pandoc method, and I drag the md file and the media folder into my Obsdian vault. How can I move the images from the media folder to the default attachment path I've set in obsidian, and have obsidian update the links to the images in the markdown file?

## **Gemini Response**
That's one of the best features of Obsidian! It's designed to handle exactly this.

As long as you **move the files inside the Obsidian app**, it will automatically find and update all the links in your markdown note.

Here is the simple, step-by-step process.

---

### 1. Configure Your Attachment Folder (If You Haven't)

First, make sure Obsidian knows where you want your attachments to live.
1.  Go to **Settings** > **Files & Links**.
2.  Find the setting **"Default location for new attachments"**.
3.  Set this to **"In the folder specified below"**.
4.  In the **"Attachment folder path"** box that appears, type the name of your attachments folder (e.g., `_attachments` or `assets`).



### 2. Move Your Images Inside Obsidian

This is the most important part. **Do not** move the files using your computer's Finder or File Explorer, as Obsidian won't know you did it.

1.  In the Obsidian file explorer sidebar (on the left), you should see your new note (`output-file.md`) and the new folder (`media`).
2.  Click the arrow to expand the `media` folder.
3.  Select all the images inside the `media` folder.
4.  **Drag and drop all of those images** directly onto the name of your default attachment folder (e.g., `_attachments`) in the sidebar.



That's it. Obsidian will move the files and instantly update your `output-file.md` to reflect the new file paths. The links will change from `![](media/image1.png)` to `![](/_attachments/image1.png)` automatically.

### 3. Clean Up

After you've moved all the images and confirmed the links work, you can safely right-click and **delete the now-empty `media` folder** to keep your vault tidy.

This video provides a great overview of how to manage images and attachments within Obsidian.
[Managing Images in Obsidian](https://www.youtube.com/watch?v=dwMqai6qy3c)

## **User Prompt**
> What if I have my _attachment folder hidden in Obsidian?

## **Gemini Response**
That's a common workflow! If your `_attachments` folder is hidden (usually by a community plugin like "File Hider"), you can't drag and drop to it.

The easiest and most "Obsidian-native" way to handle this is to use the **Move file** command.

Here's how:

1.  In the Obsidian sidebar, go into your `media` folder.
2.  **Right-click** on an image you want to move (you can also select multiple images, then right-click the group).
3.  From the context menu, select **"Move file to another folder"**.

    

4.  A pop-up (the quick switcher) will appear.
5.  Start typing the name of your hidden folder: `_attachments`.
6.  Even though it's hidden from the sidebar, it will appear in this list. Select it and press **Enter**.

Obsidian will move the file(s) to your hidden `_attachments` folder and **will still automatically update all the links** in your markdown note.

Once you're done, you can safely delete the empty `media` folder.

