# Dashboard Python Dash/Plotly

Dataset gathering all the projects from Kickstarter cowdfunding platform since 2009  
378661 projects, each with 15 variables such as country, project name, amount requested, amount raised, etc.   


## Packages installation
 
Everything is in the notebook but here's all the packages needed :  

import numpy as np  
import pandas as pd  
import dash  
from dash.dependencies import Input, Output  
import dash_core_components as dcc  
import dash_html_components as html  
#import iso3166  
import plotly.plotly as py  
import plotly.figure_factory as ff  
import plotly.graph_objs as go  
from plotly import __version__  
from plotly.offline import download_plotlyjs, init_notebook_mode, plot, iplot  
external_stylesheets = ['https://codepen.io/chriddyp/pen/bWLwgP.css']  


## Script

Description of the required operations to run the dashboard.

Open a command prompt and move to the project folder.
Run kickstarter_dash.py from this command prompt: python kickstarter_dash.py.  
Wait until the csv file is downloaded and the dashboard is built.  
When the command prompt displays:  


* Restarting with stat  
* Debugger is active!  
* Debug PIN: 627-896-911  
* Running on http://127.0.0.1:8050/ (Press CTRL+C to quit) 

 
The dashboard is ready. Copy the IP address that appears and enter it in a browser.  
Do not close the command prompt while using the dashboard.  
  
If there is a need to reload the csv, uncomment the line "#ksprojects=pd.read_csv("ks-projects-201801.csv",encoding = "utf8')".  
This allows the csv to be loaded locally (which goes much faster).
