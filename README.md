# Quantum-Machine-Learning-for-Beginners
 QML seems interesting from outside but it is complex and confusing from inside. This repo will help QML beginners in building up a bridge between these two.

## Quantum Machine Learning - First Program
1. ## Checklist
   - Ubuntu 16.04 or later
     macOS 10.12.6 or later
     Windows 7 or later
   - Python 3.5 orlater 
     - https://www.python.org/downloads/
   - Anaconda (Recommended as it has all the packages necessary for a machine learner)
     - https://www.anaconda.com/distribution/
   - Visual C++ 14.0 or above 
     - https://go.microsoft.com/fwlink/?LinkId=746572 (Visual C++ Redistributable for VS 2017)
   - Install MiKTex 
     - https://miktex.org/download (for all os)
   - Install Poppler 
     - Windows
       - http://blog.alivate.com.au/wp-content/uploads/2017/01/poppler-0.51_x86.7z
       - Extract the zip folder using 7Zip (https://www.7-zip.org/download.html) into user directory c:\Users\<user_name>\
       - Add C:\Users\<user_name>\poppler-0.51\bin to the user's path by Right click on "This PC" -> Properties -> Advanced                          System Settings -> Environment Variables
      - Linux
        - Run: ```apt-get install -y poppler-utils```
       - MacOS
         - Run: ```brew install poppler```
                     
2. ## Installing Qiskit, Qiskit Aqua
   - Create a separate environment for QML
      - ```conda create -n name_of_my_env python=3```
   - Activating the environment (for Windows OS)
     - ```  activate name_of_my_env  ```      
   - Install Qiskit
     - ```pip install qiskit qiskit-aqua qiskit-chemistry```
   
3. ## IBMQ Account Setup
   - Sign up at IBMQ ->https://quantumexperience.ng.bluemix.net/qx/login
   - After signing up, open My Account->Advanced->Regenerate->Copy API Token
   - Run the following commands:
    ``` from qiskit import IBMQ
        MY_API_TOKEN='paste your token here'
        url='https://quantumexperience.ng.bluemix.net/api'
        IBMQ.save_account('MY_API_TOKEN',url,overwrite=True)
        IBMQ.load_accounts()```

