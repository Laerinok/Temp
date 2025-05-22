# Quick Guide: Exporting Maps from .db to .png

This guide will walk you through converting your `.db` map files into `.png` images using a Python script. Don't worry if you're new to Python; we'll cover everything step-by-step.

---

### 1. Install Python

Python is the language this script is written in. Your computer needs it to run the script.

1.  **Download Python:**
    * Go to the official Python website: [https://www.python.org/downloads/](https://www.python.org/downloads/)
    * Click the "**Download Python X.Y.Z**" button for your operating system (e.g., Windows, macOS).
2.  **Run the Installer:**
    * Double-click the downloaded file (e.g., `python-X.Y.Z.exe` on Windows).
    * **Crucial for Windows:** On the very first screen, **make sure to check the box that says "Add Python X.Y to PATH"** at the bottom. This is essential for the script to work easily.
    * Click "**Install Now**" and follow the prompts.

---

### 2. Download the Program Files

Next, get the actual script and its related files.

1.  **Download VS Map Renderer:**
    * Go to the project's release page (where you originally downloaded it). Look for the "**latest release**" and download the **`.zip` file** (e.g., `vsmaptools-X.Y.Z.zip`).
2.  **Extract the Files:**
    * **Right-click** the downloaded `.zip` file.
    * Select "**Extract All...**" or "**Unzip here.**"
    * Choose a folder (e.g., create a new folder on your desktop called `Map_Converter`).
    * Inside the extracted folder, you should find `vsmaptools.py`, `requirements.txt`, and `config.json`.

---

### 3. Install Necessary Components (Dependencies)

The script needs a few extra "ingredients" to function. We install these using your computer's "command line" or "terminal."

1.  **Open Terminal/Command Prompt:**
    * **On Windows:** Click the search icon in your taskbar, type `cmd`, and press **Enter**.
    * **On Mac:** Go to "Applications" > "Utilities" > "**Terminal**," or search for "Terminal" with Spotlight (Cmd + Space).
2.  **Navigate to the Script's Folder:**
    * In the terminal window, type `cd ` (that's `cd` followed by a space).
    * Then, **drag and drop the `Map_Converter` folder** you created in Step 2 directly into the terminal window. The full path will appear.
    * Press **Enter**.
3.  **Install Dependencies:**
    * Once you're in the correct folder in the terminal, type or paste the following command and press **Enter**:
        ```bash
        pip install -r requirements.txt
        ```
    * You'll see text scrolling as your computer downloads and installs the required components. Wait until the command line becomes available again (you see the folder path or prompt).

---

### 4. Convert Your Map

Now you're ready to convert your map.

1.  **Place Your .db File:**
    * Put your **`.db` map file** (the one you want to convert) **into the same folder** as `vsmaptools.py`.
2.  **Run the Script:**
    * Go back to your terminal window.
    * Type the following command and press **Enter**:
        ```bash
        python vsmaptools.py
        ```
**IMPORTANT:** Replace the 'map_file' value in the config file  with the **exact name** of your `.db` file (e.g., `17036cd4-fd1c-4c2b-87ff-5c5e3fe6eee7.db`).
* The script will run. Once it's finished, a new **`.png` image file** (with the name defined in the config file at the 'output' value.) will appear in the same folder.
