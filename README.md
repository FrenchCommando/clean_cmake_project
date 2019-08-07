# clean_cmake_project
python script to generate skeleton for cmake project for c++

## Dependency
- python package stringcase - to convert name formats from/to pascal/snake/constant
- listed in requirement.txt
- python 3 - currently working with 3.7

## Usage
- Place the script ProjectSkeleton.py in the main project folder - which may be empty
- Run the script in cmd
  - The script will prompt a name for the new sub_project
  - Enter the project name and hit Enter

## Structure
- If not already present, a CMakeLists.txt file will be created and filled.
- googletest will be cloned in /libs/googletest
- source files are placed in the /src/ folder - with one sub-folder for each sub-project
- test files are placed in the /tests/ folder - with one sub-folder for each sub-project

##Links
- The name of the main project is retrieve from the location of the script, it is used for
  - name of the project in the main CMakeList.txt
  - guards for .h files (#define CLEAN_CMAKE_PROJECT_TOTO_H)
- The main CMakeLists.txt contains links to
  - googletest directory
  - each src and tests sub-directories
- The CMakeLists.txt from the test folder has a link to the project defined in the src folder
  - the .cpp test contains and include to the .h in the src folder

## Contribution
Anything is always welcome
