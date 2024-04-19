# Database convention and custom Python script
Do merge all databases files into single directory, the batch renaming of files must be done.
The labeling 101_1, 101_2... 102_1, 102_2... were consistent through each database, so to preserve the labling conventions,
the initials were changed to

101_1 to 201_1 for DB2, and 301_1 for DB3 so that DB can be identified while still keeping convention.
Custom python script was executed to make task faster.

```
import os

def rename_files(directory):
    # Iterate through all files in the directory
    for filename in os.listdir(directory):
        if os.path.isfile(os.path.join(directory, filename)):  # Check if it's a file
            # Extract the file extension
            _, extension = os.path.splitext(filename)
            
            # Check if the first character is '1'
            if filename[0] == '1':
                # Construct the new filename by changing the first character to '2'
                new_filename = '2' + filename[1:]
                
                # Rename the file
                os.rename(os.path.join(directory, filename), os.path.join(directory, new_filename))

# Example usage:
directory_path = "DB2_B"
rename_files(directory_path)

```
