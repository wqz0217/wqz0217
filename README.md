# Exam Score Data Analysis  

## Motivation  
The purpose of this project is to simplify the process of analyzing students’ exam scores and help teachers calculate and display important data more easily. The reason for the project comes from the widespread application of data analysis and the need from teachers to know the students’ contributions to the scores.  

## Build Status  
The project is finished, and it has been tested to work correctly.  

## Screenshots  
![image](https://github.com/user-attachments/assets/fd6d6e75-d49a-41b7-9c19-086fdc976500)
![image](https://github.com/user-attachments/assets/9c2e474a-8462-4690-9da0-f34f4184e228)
![image](https://github.com/user-attachments/assets/a678fd73-3717-4f1f-afd2-8537f7b8ce40)
![image](https://github.com/user-attachments/assets/eabcea7a-62ad-4701-9ad3-d60b587023d9)


## Tech/Framework Used  
- **Pandas**: To read and analyze the data  
- **Google Colab**: To run code online  

## Features  
In this project, students' exam scores are analyzed using:  
- Mean, Median  
- Proportion of scores over 60  
- 75th Percentile, and more  

Additionally, a menu is provided to allow users to easily obtain the desired results. Users can also specify the file name where the results will be saved.  

## Code Examples  
```python
# Calculate the proportion of scores over 60
def calcuProportionOver60(data):
    countOver60 = 0
    for num in data:
        if num > 60:
            countOver60 += 1
    proportion = countOver60 / len(data)
    return proportion
```

## API Reference  
- **`calculAverage(data)`**: Calculate the mean  
- **`calculMedian(data)`**: Calculate the median  
- **`maxValue(data)`**: Calculate the maximum value  
- **`minValue(data)`**: Calculate the minimum value  
- **`calculVariance(data)`**: Calculate the variance  
- **`calculQ3(data)`**: Calculate the 75th percentile  
- **`calcuRange(data)`**: Calculate the range  
- **`calcuProportionOver60(data)`**: Calculate the proportion of scores over 60  

## How to Use  
1. **Mount Google Drive** to the `/drive` directory, and change the current working directory to the specified folder within Google Drive using the following code:  
    ```python
    from google.colab import drive
    drive.mount('/drive', force_remount=True)
    %cd '/drive/MyDrive/Colab Notebooks/midterm/'
    ```
2. **Run the Code** and enter the file name according to the instructions.  
3. **Follow the Instructions** to enter the number corresponding to the result you want.  

## Credits  
The data set of students' scores comes from:  
[https://www.kaggle.com/datasets/lainguyn123/student-performance-factors](https://www.kaggle.com/datasets/lainguyn123/student-performance-factors)

---
<!---
wqz0217/wqz0217 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
