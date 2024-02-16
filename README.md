
# Insta-Scrapper

Hello Everyone, This is an Instagram Scrapper that is capable to Login-Logout, Searching and open disire profile, extract following information about a profile -
- User Id
- User Name
- No. of Posts
- No. of Follower
- No. of Following
- Verification status
- Public and Private status
  
It is also capable to extract following data related of post of a User - 
- Post Url
- Caption
- No. of Likes
- Posted Date
- Tagged Persons
It can also save data into excel file to further analysis purposes.

You can check Jupyter Notebook "InstaScrapper.ipynb" and Sample Excel File "Database.xlsx". 
If There is any problem in the code Please let me know.

## Usage/Examples

```python
#To Start WebDriver

driver = wdinit(obs=1)

0 --> Headless Mode
1 --> Window Mode
By Default It is 0, To pervent the intruption between the process of WebDriver

Function will return "driver"
```
```python
#To Login

login(driver, Username, Password) 
```
```python
#To get information of profile

profile dataframe, post dataframe = info(driver, profilelist, no of post, disired date)

e.g-
profile_df, post_df = info(driver, profilelist, None, 'Jan 01, 2024')
                  or
profile_df, post_df = info(driver, profilelist, 10, None)

profilelist --> It is a list of users or profiles
no of post --> How many posts data you want to extract, By default it is None
disired date --> If you want to extract posts from any date, By default it is None

Function will return two dataframe (Profile and Post).
Note-Date should be in format of 'mmm dd, yyyy'
```
```python
#To Logout

logout(driver) 
```
```python
#To close WebDriver

wdclose(driver) 
```
```python
#To Save in Excel File
save_to_excel(directory, profile dataframe, post dataframe, excel name)

e.g-

directory = r"location"
save_to_excel(directory, profile_df, post_df, 'data')

directory --> Location Where you want to save Excel File, 
```


## Lessons Learned

- Python
- Selenium
- Pandas 
- Openpyxl
- datetime


# Hi, I'm Chetan Sharma! 👋


## 🚀 About Me
I'm a Python Developer and working on Data Science, Machine Learning and Deep Learning Projects.


## License

[MIT](https://choosealicense.com/licenses/mit/)


## Authors

- [@chetan sharma](https://www.github.com/che26tan)

