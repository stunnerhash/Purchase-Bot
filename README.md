# Purchase Bot
<!--<br/><br/>
* Easy to use interface built on PyQt5
* Waits for items to restock if they are out of stock
* Optional price checker
* Lighting fast auto-checkout

## Current Functionality

## Purchase Bot Repository Link
[View The Repo Here](https://github.com/stunnerhash/Purchase-Bot/)
 -->
## Quick Install for Windows
1. Make sure your Chrome browser is updated to the latest
2. Install the latest version of [Git](https://git-scm.com/downloads) & [Python](https://www.python.org/downloads/)
3. Open Powershell as Administrator within your desired directory for the application to live.
4. Run the following commands: 
      ```
      git clone https://github.com/stunnerhash/Purchase-Bot.git
      ```
      ```
      cd Purchase-Bot
      ```
	  ```
	  Set-ExecutionPolicy RemoteSigned
	  ```
      ```
      python -m venv ./env
      ```
      ```
      ./env/Scripts/activate
      ```
      ```
      python -m pip install --upgrade pip 
      ```
      ```
      pip install -r requirements.txt
      ```
      ```
      pip install chromedriver_py 
      ```
4.1 If you encouter any errors while running ./env/scripts/activate use command:
```
setExecutionPolicy RemoteSigned
```
4.2 If you encounter any errors during installation, please consider the following:
    * If you get a red text error remove and you previously installed pyqt5 or lxml on your python, remove the versions from the **requirements.in** for both lxml and pyqt5, then run the following commands:
    ```
    pip install pip-tools==5.5.0
    ```
    ```
    pip-compile --generate-hashes --no-index --output-file=requirements.txt requirements.in
    ```
    ```
    pip install -r requirements.txt
    ```
    * If you get an error with red text run the following: 
     ```
     pip install pycryptodomex
     ```
5. Run the following command:
   ```
   python app.py
   ```

## Quick Install for Mac
**It is highly recommended you install brew and update python3 to latest version**

1. Make sure your Chrome browser is updated to the latest
2. Run the following commands: 
      ```
      git clone https://github.com/stunnerhash/Purchase-Bot.git
      ```
      ```
      cd Purchase-Bot
      ```
      ```
      python3 -m venv ./env
      ```
      ```
      source env/bin/activate
      ```
      ```
      python3 -m pip3 install --upgrade pip 
      ```
      ```
      pip3 install -r requirements.txt
      ```
3. If you encounter any errors during installation, please consider the following:
    * If you get a red text error remove and you previously installed pyqt5 or lxml on your python,  remove the versions from the **requirements.in** for both lxml and pyqt5, then run the following commands:
    ```
    pip3 install pip-tools==5.4.0
    ```
    ```
    pip-compile --generate-hashes --no-index --output-file=requirements.txt requirements.in
    ```
    ```
    pip3 install -r requirements.txt
    ```
    * If you get an error with red text run the following: 
     ```
     pip3 install pycryptodomex
     ```
4. Run the following command:

   ```
   python3 app.py
   ```


## Windows FAQs
To resume working on the bot for testing after closing powershell, navigate again to the folder and run the following commands:
  ```
  ./env/Scripts/activate
  python app.py
  ```
<!-- 

## Contributing
This project uses pip-compile with the --generate-hashes flag to validate dependencies via checksums. This helps prevent updates to existing package versions on PyPI from adding new code to our project. When changing requirements, make updates in the requirements.in file, then compile using the command below to update requirements.txt before committing.
```
pip-compile --generate-hashes --no-index --output-file=requirements.txt requirements.in
```
If you receive an error when running this command related to pinning a version of pip, make sure your system or virtualenv pip version is up to date by running the following command:
```
python -m pip install --upgrade pip
```
 -->
