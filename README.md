# ⚡ electric-school-bus-adoption-clustering - Analyze Electric Bus Adoption Patterns  

[![Download Now](https://img.shields.io/badge/Download-Get%20Files-blue?style=for-the-badge&logo=github)](https://github.com/Daunting-beefloin312/electric-school-bus-adoption-clustering)

## 🔍 What This Application Does  

This application uses unsupervised learning methods to study how electric school buses are adopted. It groups data based on similarities without needing labeled examples. The analysis focuses on social, economic, and environmental features to find patterns. It also reduces complex data to simpler forms to make it easier to understand. This helps users explore how different factors influence electric bus adoption.  

## 🖥️ System Requirements  

- Windows 10 or later  
- 8 GB RAM or more  
- At least 500 MB free disk space  
- Internet connection for initial download  
- Python 3.8 or newer installed  

If you do not have Python, the setup section will guide you on installing it.  

## 🚀 Getting Started: Download and Prepare  

Start by downloading the application files. Use the link below to go to the GitHub page where you can get everything you need.  

[![Download Application](https://img.shields.io/badge/Download-Get%20Files-green?style=for-the-badge&logo=github)](https://github.com/Daunting-beefloin312/electric-school-bus-adoption-clustering)

1. Click the link above to visit the GitHub page.  
2. On the page, find the green “Code” button near the top right.  
3. Click the button and select “Download ZIP”.  
4. Save the ZIP file on your computer, such as the Desktop or Downloads folder.  

## 📂 Unpack the Files  

1. Find the ZIP file you downloaded.  
2. Right-click the file and select “Extract All”.  
3. Choose a destination folder where you want the files.  
4. Click “Extract”. This will create a folder with the application files inside.  

## 🐍 Installing Python and Dependencies  

If you do not have Python installed, follow these steps:  

1. Open your internet browser and visit https://www.python.org/downloads/windows/  
2. Select the latest stable Python version compatible with Windows.  
3. Download the Windows installer (usually named “python-3.x.x-amd64.exe”).  
4. Run the installer file.  
5. **Important:** On the first installer screen, check the box “Add Python 3.x to PATH”.  
6. Click “Install Now” and wait until the installation finishes.  

After installing Python, you need to install required Python packages. These packages provide the tools the application uses to analyze data.  

1. Open the “Command Prompt” by pressing Windows + R keys, typing `cmd`, and pressing Enter.  
2. In the Command Prompt window, type the following command and press Enter:  

   ```  
   pip install -r requirements.txt  
   ```  

This command reads a list of needed packages from the application folder and installs them automatically.  

If you get an error, make sure you are inside the folder where you extracted the files. You can change the folder in Command Prompt by typing:  

```  
cd path\to\your\application\folder  
```  

Replace `path\to\your\application\folder` with the actual folder path.  

## ⚙️ Running the Application  

1. Open the folder where you extracted the files.  
2. Find the file named `run_app.bat` or `start_app.bat`. This is a simple script to launch the application without typing commands.  
3. Double-click this file to run the application. A new window or command prompt should open showing progress and results.  

If there is no `.bat` file, follow these steps using Command Prompt:  

1. Open Command Prompt (Windows + R, then `cmd`).  
2. Change to the folder with the application files:  

   ```  
   cd path\to\your\application\folder  
   ```  

3. Run the application by typing:  

   ```  
   python main.py  
   ```  

Replace `main.py` with the actual main script if named differently.  

## 🔬 Understanding What Happens  

The app takes data about electric school bus use, school locations, income levels, weather, and other factors. It finds groups, or “clusters,” of similar places. For example, it might find that areas with high income and mild weather adopt buses faster.  

The app also uses dimensionality reduction methods to shrink complex data into 2D or 3D views. This lets you see the groups in easy-to-understand charts.  

Results appear as simple tables and graphs in the app window. You can save these charts as files to your computer.  

## 🗂️ Files Included  

- `main.py`: The main program file that starts the analysis.  
- `requirements.txt`: List of Python packages required.  
- `data/`: Folder that holds input data used by the program.  
- `output/`: Folder where the app saves charts and results after it runs.  
- `README.md`: This instructions file.  
- `.bat` launch script(s) for easy starting (if included).  

## 💡 Tips for Best Use  

- Keep your data folder updated. Add new data files in the same format to analyze fresh information.  
- Run the app from the command prompt if you do not see results from the batch file.  
- Check the output folder after the run to find charts and reports.  
- Close the app window when finished to release memory and resources.  

## 📥 Download Link  

Use this link to get the application files and updates:  

https://github.com/Daunting-beefloin312/electric-school-bus-adoption-clustering  

Visit the page, then download the ZIP file with all code and data.  

## ⚙️ Troubleshooting  

- If Python commands do not work, check that Python is added to your system PATH.  
- Errors about missing packages mean dependencies did not install. Retry `pip install -r requirements.txt`.  
- If you see permission errors, run Command Prompt as Administrator.  
- For unexpected crashes, try restarting your computer and running again.  
- Detailed error messages appear in the Command Prompt window and can guide fixes.  

## 📚 Additional Resources  

This application uses common Python tools:  

- scikit-learn: for clustering and data analysis  
- umap-learn: for dimensionality reduction  
- pandas and numpy: for data handling  
- matplotlib or seaborn: for charts and graphs  

Learning the basics of Python and these tools may help if you want to modify or extend the program.  

---

[![Download on GitHub](https://img.shields.io/badge/Download-GitHub%20Page-grey?style=for-the-badge&logo=github)](https://github.com/Daunting-beefloin312/electric-school-bus-adoption-clustering)