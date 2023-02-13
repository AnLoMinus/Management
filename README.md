# Management
## Management System Directory Structure

The main directory is `Management` and it contains five subdirectories:

- `Planning`
- `Organizing`
- `Leading`
- `Controlling`
- `Decision Making`

For each of the subdirectories, there are specific subfolders created under them, as specified in the arrays:

- `planning_folders`
- `organizing_folders`
- `leading_folders`
- `controlling_folders`
- `decision_making_folders`

The code checks if each directory already exists using the `os.path.exists()` method. If the directory does not exist, the code creates it using the `os.makedirs()` method.

```python
import os

directory = "Management"
subdirectories = ["Planning", "Organizing",
                  "Leading", "Controlling", "Decision Making"]

# create main directory
if not os.path.exists(directory):
    os.makedirs(directory)

# create subdirectories
for subdir in subdirectories:
    subdirectory = directory + "/" + subdir
    if not os.path.exists(subdirectory):
        os.makedirs(subdirectory)

planning_folders = ["Strategic Planning",
                    "Tactical Planning", "Operational Planning"]
organizing_folders = ["Resource Allocation",
                      "Role and Responsibility Definition", "Process Definition and Implementation"]
leading_folders = ["Leadership Development",
                   "Team Management", "Communication and Motivation"]
controlling_folders = ["Performance Management",
                       "Risk Management", "Quality Management"]
decision_making_folders = [
    "Problem Solving", "Decision Making Methodologies", "Decision Making Best Practices"]

# create subfolders for Planning
for folder in planning_folders:
    subfolder = directory + "/" + "Planning" + "/" + folder
    if not os.path.exists(subfolder):
        os.makedirs(subfolder)

# create subfolders for Organizing
for folder in organizing_folders:
    subfolder = directory + "/" + "Organizing" + "/" + folder
    if not os.path.exists(subfolder):
        os.makedirs(subfolder)

# create subfolders for Leading
for folder in leading_folders:
    subfolder = directory + "/" + "Leading" + "/" + folder
    if not os.path.exists(subfolder):
        os.makedirs(subfolder)

# create subfolders for Controlling
for folder in controlling_folders:
    subfolder = directory + "/" + "Controlling" + "/" + folder
    if not os.path.exists(subfolder):
        os.makedirs(subfolder)

# create subfolders for Decision Making
for folder in decision_making_folders:
    subfolder = directory + "/" + "Decision Making" + "/" + folder
    if not os.path.exists(subfolder):
        os.makedirs(subfolder)
```

This code creates a directory structure for a management system.  
The main directory is "Management" and it contains five subdirectories: "Planning", "Organizing", "Leading", "Controlling", and "Decision Making".

For each of the subdirectories, there are specific subfolders created under them, as specified in the arrays planning_folders, organizing_folders, leading_folders, controlling_folders, and decision_making_folders.

Before creating any directory, the code checks if it already exists using the os.path.exists() method.  
If the directory does not exist, the code creates it using the os.makedirs() method.

