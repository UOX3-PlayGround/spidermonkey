# Embedded Java Script
This is based of of SpiderMonkey 1.7, but has been modified to include files needed minimal embedding purposes.  
The build setups generate a static library for only embedding purposes.  
See [SpiderMonkey](https://spidermonkey.dev) for original files.
## Building
### Integrated Development Environments
#### XCode and VS2022
Project files are located in the ./ide/ directory
### CMake
1. Create a build location  
   - Enter:  `mkdir build`  
2. Move to that locations  
   - Enter:  `cd build`  
3. Create the make files   
   - **Windows**  (from a Developers command prompt)  
      - Enter:  `cmake .. -DCMAKE_BUILD_TYPE=Release -G"NMake Makefiles"`  
    - **macOS**  
      - Enter:  `cmake .. -DCMAKE_BUILD_TYPE=Release -G"Unix Makefiles"`  
    - **All Other Operation Systems**  
      - Enter:  `cmake .. -DCMAKE_BUILD_TYPE=Release`  
4. Build the system entering:  `cmake --build . --config Release`  
5. The resulting product will be in the current (build) directory    
 