# Practical-Application-1
 Repo of PCMLAI Practical application Module 5 assignment files

## Description of files in the repo :
 - 'coupons.csv' :  dataset file used for practical application 1
 - 'in_vehicle_coupons.ipynb' : solution file for the assignment.
#### Bar Coupon graphs
 - sns.barplot(x='maritalStatus', y='count', hue='maritalStatus', data=marital_counts, palette='coolwarm', legend=False)
<img width="716" alt="Screenshot 2024-10-08 at 12 03 12 AM" src="https://github.com/user-attachments/assets/4ca778f6-2f69-4934-bff3-5729235f4138">

 - sns.barplot(x='Bar', y='count', hue='Bar', data=bar_counts, palette='plasma', legend=False)
 <img width="743" alt="Screenshot 2024-10-08 at 12 02 57 AM" src="https://github.com/user-attachments/assets/ed9a6546-fb66-4684-8c94-0534c302d946">

 - sns.barplot(x='age', y='count', hue='age', data=age_counts, palette='viridis', legend=False)
 <img width="726" alt="Screenshot 2024-10-08 at 12 02 27 AM" src="https://github.com/user-attachments/assets/23f98811-ac10-4770-8b1a-07451ed7fc52">

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

### Unemployed age group who depend on 'Carry out and Take away' coupons
 - data_unemployed_carryout = data_carryout[(data_carryout['occupation'] == 'Unemployed')]
 - sns.histplot(data_unemployed_carryout['age'], bins=5, kde=False, color='blue')
<img width="910" alt="Screenshot 2024-10-07 at 10 57 30 PM" src="https://github.com/user-attachments/assets/4b291346-9124-42b3-8e2f-d13f709c1c59">







