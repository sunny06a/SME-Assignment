# Space-Invaders

## Overview

This project is a simple implementation of the classic arcade game Space Invaders using SFML 2.6.1.


## 1) Installation & Setup

Follow these steps to set up the project on your local machine:

1. **Cloning the Repository**: 
   - Forked the [GitHub](https://github.com/rnv10/SME-Assignment) repository using GitHub and then cloned the forked version on a local device using the following command:
     ```sh
     git clone https://github.com/sunny06a/SME-Assignment
     ```

2. **Adding SFML 2.6.1 Files**:
   - Downloaded SFML 2.6.1 from the [official website](https://www.sfml-dev.org/download/sfml/2.6.1/), specifically the Visual C++ 15 (2017) - 64-bit version.
   - Followed the setup guide provided in the Notion to add the `include` and `lib` folders to the project.

3. **Building the Project**:
   - Built the project using Visual Studio Community.

## 2) Bug Fix

There were many warnings and 3 errors:
1. **Locate the Bug**:
   - The bug can be found in `space_invasion/header/Player/PlayerController.h` where undefined classes are used.

2. **Solution**:
   - In `PlayerController.h`, defined the two classes `PlayerModel` and `PlayerView` using forward declaration:
     ```cpp
     class PlayerModel;
     class PlayerView;
     ```

3. **Execution**:
   - After fixing the bug, the code executed successfully.
   ![image](https://github.com/sunny06a/SME-Assignment/assets/83196848/dca15a5e-4fc5-4e85-b0f3-9998d7b677ab)
