# GitHub Analyzer Project

This project creates a Command Line Interface (CLI) that displays relevent metrics related to a GitHub user! The metrics are: total number of repositories, most frequently used programming language, most starred and forked repositories, and a user's weekly commit frequency.


## Set Up 
Start by **cloning this repository**. 
Take a look at the technologies and dependencies required to successfully run the CLI locally!

### Requirements 
This project was developed with the following: 
| Technology | Version |
| ------------- | ------------- |
| Python | v3.10+  |
| Pip  | v23.1+  |


### Dependencies 
Run the following in command line to install the necessary dependencies:


```
pip install requests  
```
```
pip install prettytable
```
```
pip install matplotlib
```
```
pip install argparse
```
```
pip install colored
```


## Run 
Now that set up is complete, you can run the CLI! Follow these steps: 
1. Navigate to the cloned repository directory in command line, if you haven't already.
2. Open `metrics_test.py`. Enter your own GitHub credentials-- your username and access token. Update the `access_token` and `user` fields in this file. 
3. Run the following script, entering in the GitHub username you would like to see metrics for. `github_username` is a required argument

```
python3 metrics.py <github_username>
```

#### Note: 
This CLI uses `argparser`. To see the acceptable arguments and their description, run the following command with the 'help' flag: 
```
python3 metrics.py -h
```
As you will see from the output, the CLI also accepts two optional flags: 

` --save` : optional flag to save data retrieved

`--gr` : optional flag to generate and save graph image


## Test
The unit tests are written in `metrics_test.py`. 
Run the following command to run the tests: 
```
python3 -m unittest metrics_test.py
```



## Helpful Links



Code Documentation 