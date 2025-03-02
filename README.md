# Python Virtual Environment Setup Guide

This guide explains how to set up a virtual environment in Python, generate a `requirements.txt` file, and manage dependencies. This is useful for keeping project dependencies isolated and organized.

---

## **1. Create a Virtual Environment**

Navigate to your project folder and run:

```sh
python -m venv myenv
```

Here, `myenv` is the name of your virtual environment. You can choose any name.

---

## **2. Activate the Virtual Environment**

### **On Windows (Command Prompt):**

```sh
myenv\Scripts\activate
```

### **On macOS/Linux:**

```sh
source myenv/bin/activate
```

Once activated, you will see `(myenv)` before your command prompt, indicating that the virtual environment is active.

---

## **3. Install Dependencies**

After activation, install required dependencies:

```sh
pip install package_name
```


## **4. Generate a ****\`\`**** File**

To save all installed dependencies, run:

```sh
pip freeze > requirements.txt
```

This will create a `requirements.txt` file listing all dependencies.

---

## \*\*5. Install Dependencies from \*\*\`\`

If you want to set up the same environment on another system, run:

```sh
pip install -r requirements.txt
```

This installs all dependencies listed in the file.

---

## **6. Deactivate the Virtual Environment**

When you're done, deactivate it by running:

```sh
deactivate
```

Your terminal will return to the normal prompt.

---

## **7. Delete the Virtual Environment (If Needed)**

To remove the virtual environment, simply delete the folder:

```sh
rm -rf myenv  # macOS/Linux
rd /s /q myenv  # Windows
```

---

This guide should help beginners understand and manage virtual environments easily. If you have any issues, feel free to ask! 😊

