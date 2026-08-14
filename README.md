
filePath = matlab.desktop.editor.getActiveFilename;
slash = zeros(length(filePath),1);
for i = length(filePath):-1:1
    if filePath(i) == '\'
        slash(i,1) = 1;
    end
end
%filePath = filePath(1:length(slash) ); cd (filePath);
folderPath = fileparts(filePath);
cd(folderPath);


 


 
% rootpathData = uigetdir(pwd, ['Go to your downloaded path and then ' ...
%     'select Day3_Lab_SaugatB\dataset']);
addpath(fullfile(pwd,'dataset'));
