# Step 1. What is docker?  
Docker is a way to contianerize your applications/services. It's like taking a function that does two things and making it into two functions that each do one thing. One of the key benefits is that they are lighter than virtual machines. So you can run many more contianers on a host than you can virtual machines. 
Docker is just the front end to a myriad of container technologies that are offered to users via the linux kernel. Docker uses cgroups and other isolation tech found in the kenrel to do what it does. Indeed, before docker, you could do most everything docker could do when it was released if you were an uber linux nerd but docker just made things a lot easier and acutally useful to the rest of us. 

# Step 2. Enough talk, let's dockerize something already!  

(here you'll just git clone the repo, but it's good to have some practice so if you don't want to clone it follow along)  

``` mkdir $HOME/pywebapp```    
```cd $HOME/pywebapp```  
```pipenv --python 3.5 #could also do 3.6 if you're on it```  
```pipenv install asyncpg aiohttp```  
Verify things work by trying to instantiate the modules you just installed  
```python3 -m aiohtt ```    
```python3 -m asyncpg```  
if you see this: 
```bin/python3: No module named asyncpg.__main__; 'asyncpg' is a package and cannot be directly executed```  
```bin/python3: No module named aiohttp.__main__; 'aiohttp' is a package and cannot be directly executed```  
Then the modules are installed and usable. Yay!
