## Git from Scratch 

#### Git bash

### 1. Start a new repository:

There are two ways to begin with an new file on your own workspace

- Begin on Github.com 
        
    Build a new folder "new", and then go to your git bash **Home directory**
    
```{r}
git clone http://github.com/YourAccount/new.git 
cd ~/new

```

- Begin on your own workspace 

```{r}
mkdir new
cd ~/new 

echo # gitCommand >> README.md
git init
git add README.md
git commit -m "first commit"
git remote add origin https://github.com/travisho0014/gitCommand.git
git push -u origin master

```

### 2. Set the connection  


```{r}
git remote add origin http://github.com/YourAccount/new.git
```

set the tag **origin** = your github location, then your can use origin instead of long url.

```{r}
git remote 
git remote -v
```

See current defined index. If you want to remove defined index, then 

```{r}
git remote remove origin 
/* or */
git remote rm origin
```

### 3. Define current working index

```{r}
git add  .      // add file 
git add -u      // update 
git add -A      // add and update
```

use commit to finalize the index 

```{r}
git commit 
git commit -m "message"
```

###4. Synchronize with github 

```{r}
git pull origin 
/* or */
git pull 
```

###5. Update the workingspace file 

```{r}
git push origin master 
/* or */
git push origin branceName 
```




