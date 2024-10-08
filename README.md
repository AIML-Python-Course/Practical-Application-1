# Practical-Application-1
 Repo of PCMLAI Practical application Module 5 assignment files

## Description of files in the repo :
 - 'coupons.csv' :  dataset file used for practical application 1
 - 'in_vehicle_coupons.ipynb' : solution file for the assignment.

## Independent Investigation
 - Using the bar coupon example as motivation, explored 'Carry out & Take away' coupon group
  
### explore 'Carry out & Take away' coupon group
 - data_carryout = clean_data[(clean_data['coupon'] == 'Carry out & Take away') & (clean_data['Y'] == 1)]
### Carryout Coupon Acceptance by Occupation
 - sns.countplot(x='occupation', data=data_carryout, hue='occupation', palette='coolwarm', dodge=False, legend=False)
<img width="987" alt="Screenshot 2024-10-07 at 10 58 10 PM" src="https://github.com/user-attachments/assets/daf0a671-627a-4e3d-a70b-a9cb531a3b41">

### Histogram of age distribution for accepted carryout coupons
 - sns.histplot(data_carryout['age'], bins=8, kde=False, color='green')
<img width="961" alt="Screenshot 2024-10-07 at 10 57 53 PM" src="https://github.com/user-attachments/assets/4606b6c6-0125-4bc0-806c-3996a4bf64a8">

# Unemployed age group who depend on 'Carry out and Take away' coupons
 - data_unemployed_carryout = data_carryout[(data_carryout['occupation'] == 'Unemployed')]
 - sns.histplot(data_unemployed_carryout['age'], bins=5, kde=False, color='blue')
<img width="910" alt="Screenshot 2024-10-07 at 10 57 30 PM" src="https://github.com/user-attachments/assets/4b291346-9124-42b3-8e2f-d13f709c1c59">







