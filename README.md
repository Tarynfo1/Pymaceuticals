# Pymaceuticals

Please see Pymaceuticals Final for final working code for this challenge. Please note at output 10 there is there an error in outputting the correct sentence structure for calculating the IQR, the caluclation is correct however the output could not be solved in time for the challenge completion. 

Pymaceuticals challenge

## Acknowledgements

The code implementation for for formatting the decimal points through the code  was provided by https://thepythonguru.com/python-string-formatting/. The provided code snippet helped in correctly formatting the decimals throughout the code.

### Code Snippet

``
' ...

' Generate a summary statistics table of mean, median, variance, standard deviation, and SEM of the tumor volume for each regimen
' Use groupby and summary statistical methods to calculate the following properties of each drug regimen:
' mean, median, variance, standard deviation, and SEM of the tumor volume. 
'mean = Clean_df.groupby("Drug Regimen")["Tumor Volume (mm3)"].mean().map('{:.2f}'.format)

' ...


The insights and code helped enhance the functionality and efficiency of the assignment. 

The code implementation for formatting the layout of the bar graph and scatter plots was assisted by https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.tight_layout.html. The provided code snippet helped in fixing the formatting to match the example.

### Code Snippet

``
' ...

'Generate a bar plot showing the total number of rows (Mouse ID/Timepoints) for each drug regimen using Pandas.
'drug_reg = Clean_df.groupby("Drug Regimen")
'drug_count = pd.DataFrame(drug_reg["Drug Regimen"].count())
'drug_reg_bar = drug_count.plot(kind='bar', color="steelblue", figsize=(7,4))

' ...

The insights and code helped enhance the functionality and efficiency of the assignment. 


The code implementation for linear regression was assisted by https://stackoverflow.com/questions/48370562/how-to-add-regression-line-and-regression-line-equation-on-graph. The provided code snippet helped in using this as a template for my own formatting.

### Code Snippet

``
' ...

'# Create a linear regression model for mouse weight and average observed  tumor volume for the entire Capomulin regimen
'vc_slope, vc_int, vc_r, vc_p, vc_std_err = st.linregress(capo_mice_weight, capo_mice_tumor_vol)
'vc_fit = vc_slope * capo_mice_weight + vc_int

' ...

'The insights and code helped enhance the functionality and efficiency of the assignment. 
