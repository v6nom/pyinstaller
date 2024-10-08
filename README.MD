<p align="center">🪐 PyInstaller Guide 🪐</p>
<br><br>

<p align="center"> <strong> This repository explains how to use PyInstaller to convert Python scripts into standalone executables (.exe files). <br><br> With PyInstaller, you can secure and distribute your Python programs with ease. <br><br><br> </strong> </p> <br>
<p align="center">📀 Example Scripts 📀</p>
<p align="center"><strong><i>Here are some example scripts that demonstrate how PyInstaller works:</i></strong></p>
<br><br>

hello_world.py
<p align="center"><strong><i>This is a simple Python script that prints "Hello, World!" to the console.</i></strong></p>

<pre>
<code>
print("Hello, World!")
</code>
</pre>
<br><br>

complex_script.py
<p align="center"><strong><i>This is a more complex script that could include external dependencies and requires additional considerations when converting to an executable.</i></strong></p>

<pre>
<code>
import sys

def main():
    print(f"Arguments: {sys.argv}")

if __name__ == "__main__":
    main()
</code>
</pre>
<br><br>

<p align="center">🛠️ How to Convert a Python Script to an Executable 🛠️</p>
<br><br>

<p align="center"><strong><i>Follow these steps to convert your Python script into an executable:</i></strong></p>
<br><br>

Navigate to the directory containing your script:

<pre>
<code>
cd path/to/your/script
</code>
</pre>
Run PyInstaller to create the executable:

<pre>
<code>
pyinstaller --onefile hello_world.py
</code>
</pre>
<br><br>

<p align="center">🔒 PyInstaller Settings 🔒</p>
<br><br>

--key Setting
<p align="center"><strong><i>The `--key` setting in PyInstaller is used for encryption. It specifies a key to encrypt the content of the bundled executable.</i></strong></p>
<br><br>

<p align="center"> This can be useful if you need to protect the source code or sensitive data. <br><br> </p>
Example usage:

<pre>
<code>
pyinstaller --onefile --key YOUR_SECRET_KEY your_script.py
</code>
</pre>
<p align="center"><strong><i>In this command, `YOUR_SECRET_KEY` is a string you provide. PyInstaller will use this key to encrypt the content of the executable, making it harder to reverse-engineer.</i></strong></p>
<br><br>

<p align="center">README.md inspired by https://github.com/billythegoat356/</p>
