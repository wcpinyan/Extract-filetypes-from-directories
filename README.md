# Python program to walk directories and copy files of interest to a common directory
## [A valuable Website for File/Directory (Python)...thanks Vuyisile Ndlovu ](https://realpython.com/working-with-files-in-python/#copying-moving-and-renaming-files-and-directories)

### Background: 
    Recently my wife purchased a download of embroidery files for her 
    BabyLock embroidery machine.  The files were downloaded as several 
    Zip files separated by alphabetic devisions (A-C.zip, D-G.zip, etc.)
    
    Inside of each top level Zip files were combinations of directories, 
    other zip files and, possibly the particular files suitable for her 
    machine(.PES).  However, along with the .PES files were the 
    equivalent number of other file extensions that were for 7 or 8 
    other embroidery machine brands and, hence were not needed or wanted.
    
    I devised this program to recursively call functions to walk from the 
    top level of zip files down each sub-level to the very bottom of the 
    tree extracting only the .PES files and putting them in a new top level 
    directory (PESFiles).  Each Zip file name was used to create a directory 
    o store the appropriate files to pertinent groups...if the zip file was 
    named cuteBunnies.zip, a directory named cuteBunnies was created to accept 
    the embedded files for that zip.
    
    This top level file should wind up in the c:\users\yourname\ location on a 
    Windows machine.  Have not tried on my Mac.
    
    I then copied the new top level directory and all included files of interest 
    to a DVD for transfer to her PC and to allow archiveing for her sanity.
    Yes, could have transferred over the wire, but she has a library of DVDs for
    her backup.
    
## Process
1. Download Anaconda (if not installed already.) Python 3 is required.
1. Copy this file to a known location (e.g. c:\users\yourname\)
1. open Jupyter Notebook and open this file.
1. Change the occurances of PES to the file extension of interest...
    or add fnmatches for directories, filenames or extensions as desired for your purpose.
1. IMPORTANT! For testing, uncomment the print statements and comment the "handle" statements to 
    verify that it is working.  This will show what is going to happen without actually writting anything
    to your harddrive.  If staisfied, turn the "handle" statements back on.
1. Run the cell below and watch the magic in your file explorer.
