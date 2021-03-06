## data visualization cheatsheet

### [heroku, flask, plotly, python, dash]

### data visualization article (plotly)
- https://towardsdatascience.com/build-a-web-data-dashboard-in-just-minutes-with-python-d722076aee2b

```python 
import plotly.express as px
fig = px.scatter(all_teams_df[all_teams_df.group == 'NOP'], x='min_mid', y='player', size='shots_freq', color='pl_pps')
fig.show()
```


### deploy data visualization online (heroku)
- https://medium.com/@austinlasseter/how-to-deploy-a-simple-plotly-dash-app-to-heroku-622a2216eb73
  - goto https://dashboard.heroku.com/apps
  - click "new" -> "create new app"
  - give it an app-name
  - click "create app"
  - under "deployment method" select "github"
  - log into your github account (if needed) and select the repo you need (i.e. dash_test) then click "connect"
  - under "manual deploy" click "deploy branch"

- You'll need the following files in a github repository (i.e. https://github.com/sho-portfolio/dash_test):
  - app.py (your python code)
  - Procfile (no idea what this)
  - requirements.txt (your pip installation file) 
  
 - https://signup.heroku.com/account
 - instructions to install heroku CLI: https://devcenter.heroku.com/articles/heroku-cli
 

### deploy data visualization to html automatically
- https://towardsdatascience.com/how-to-create-a-plotly-visualization-and-embed-it-on-websites-517c1a78568b
```python
import plotly.io as pio
pio.write_html(fig, file=’index.html’, auto_open=True)
```

