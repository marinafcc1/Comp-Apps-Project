# Comp-Apps-Project

The MATLAB program is a machine learining trainer for ECG signals to diferentiate arrythmias from normal ECGs. 
When running ECG_analyzer, the program will open two new tabs, which loads the data into the MATLAB path and creates variables that will be used later in the program (see following lines)

if ~isfile('PhysionetData.mat')
    ReadPhysionetData         
end
load PhysionetData


The program only analyzes 1400 files, not the entire database, it has a machine learning training window and will produce a confusion chart.

The trained program will be saved into a new file, which can be used to upload new files later through the ECG_newfile_input (Include file folder in path).
