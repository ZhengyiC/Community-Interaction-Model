Main files to run:
    gLV simulation: diffConditions.ipnb
    data normalization: d9_1_2TransDataWithNorm.ipynb
    run linear regression models: runModels.ipynb


1.Simulate raw data from the gLV model:
    run diffConditions.ipynb
    choose runing options (comment / uncomment sessions)
    set conditions in the last few sessions based on options you want to run 
    skip if you have raw experimental data 
    
2. data normalization:
    run d9_1_2TransDataWithNorm.ipynb
    specify the name of raw data file you want to normalize and normalization mode (z-score/ centralize around means)
    the normalized file will be save in interm folder
    skip if you do not want to normalize the data
    
3. run linear regression model:
    if experimental data used, save the raw data in rawData folder as csv file containing n*m mitrices data where n= number of training set and m = number of species in the experiment
    run runModels.ipynb
    see the last session for examples of running normalized and non-normalized data 
    output interaction coefficient can be found in the output folder
    