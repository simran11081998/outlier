WHAT IS OUTLIER?
An outlier is an observation that lies outside the overall pattern of a distribution. 
Usually, the presence of an outlier indicates some sort of problem. 
This can be a case which does not fit the model under study, or an error in measurement.

HOW TO REMOVE OUTLIERS?
One of the method is row removal by IQR(Inter Quartile Range)

Find Q1=(n+1)/4 th term (QUARTILE 1)
Find Q3=3(n+1)/4 th term (QUARTILE 3)
IQR(Inter Quartile Range) = Q3 - Q1
Find Min and Max
Min = Q1 - 1.5*IQR
Max = Q3 + 1.5*IQR
Values outside range(Min,Max) are outliers
and they are removed through this package

You just need to write in cmd line:
python outlier.py dataset.csv newfile.csv

Now open newfile.csv to note result