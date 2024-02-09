
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

wdinit(obs=1)

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

info(driver, profilelist noofpost)

profilelist --> It is a list of users
noofpost --> No of post in integer to extract data

Function will return two dataframe (Profile and Post).
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

save_to_excel(directory, profile_dataframe, post_dataframe)

directory --> Location Where you want to save Excel File, 
```


## Lessons Learned

- Python
- Selenium
- Pandas 
- Openpyxl


# Hi, I'm Chetan Sharma! 👋


## 🚀 About Me
I'm a Python Developer and working on Data Science, Machine Learning and Deep Learning Projects.


## License

[MIT](https://choosealicense.com/licenses/mit/)


## Authors

- [@chetan sharma](https://www.github.com/che26tan)

