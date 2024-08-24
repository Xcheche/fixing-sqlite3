# SQLite Database Management in Django

## 1. Downloading and Setting Up SQLite Binaries

**Download SQLite:**
1. Go to the [SQLite Download Page](https://sqlite.org/download.html).
2. Download the `sqlite-tools` zip file for Windows.

**Extract and Set Environment Variables:**
1. Extract the contents of the downloaded zip file to a directory (e.g., `C:\sqlite`).
2. Add the directory to your system’s `PATH` environment variable:
   - Right-click on `This PC` or `My Computer`, then click on `Properties`.
   - Click on `Advanced system settings` and then on `Environment Variables`.
   - Under `System variables`, find the `Path` variable, select it, and click `Edit`.
   - Click `New`, and add the path to the directory where you extracted the SQLite binaries (e.g., `C:\sqlite`).
   - Click `OK` to save the changes.

## 2. Backing Up Your SQLite Database

**Command to Backup Database:**
1. Open a command prompt or terminal in your Django project directory.
2. Run the following command to back up your database:
   ```bash
   sqlite3 db.sqlite3 ".backup db_backup.sqlite3"
## Creates New Database
   python manage.py migrate 
##  Copies the dumped database
copy db_backup.sqlite3 db.sqlite3


