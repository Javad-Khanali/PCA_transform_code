# PCA_transform_code
Here is a code I wrote to don't use the transform function of PCA!

I used the breast cancer data of sklearn library.
The data was converted into pandas data-frame format and its features were standardized. 
Then I fitted a PCA model to it; however, I didn't use the "pca_model.transform(X_train)" code and instead, I wrote the code inspiring from the PCA formula.
For each row of the data frame, the values of each feature are multiplied by the weight of that feature determined by PCA (components_).
the multiplication results are summed column-wise to form a value that corresponds to component 1 for row 1.
The algorithm continues row-wise to find all the component 1 values. 
the code is written for a two-component model but it can be extended to the other component numbers. 
