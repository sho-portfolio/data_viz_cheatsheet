# data_viz_cheatsheet

# heroku, flask, plotly, python

# article that got me started (plotly data viz)
## https://towardsdatascience.com/build-a-web-data-dashboard-in-just-minutes-with-python-d722076aee2b

# article that showed me how to easily make my data-viz avaikable on the web
## https://medium.com/@austinlasseter/how-to-deploy-a-simple-plotly-dash-app-to-heroku-622a2216eb73


# used jupyter notebooks to test

# but to deploy am using heroku (will try aws later)

# for heroku
[1] create an account on https://signup.heroku.com/account
[*2] install the heroku cli and git (if needed): goto terminal and type: brew tap heroku/brew && brew install heroku
* instructions are here: https://devcenter.heroku.com/articles/heroku-cli
* you need the cli as on a free heroku account you can only deploy to heroku via git
[3] goto https://dashboard.heroku.com/apps
[3.1] click "new" -> "create new app"
[3.2] give it an app-name
[3.3] click "create app"
[3.4] under "deployment method" select "github"
[3.5] log into your github account (if needed) and select the repo you need (i.e. dash_test) then click "connect"
[3.6] under "manual deploy" click "deploy branch"


## once installed - login to heroku via terminal: > heroku login -i or heroku login (use this if you let apple set a secure pasword for you and dont know what it is!)
*2: optional - can use the method in step 3 instead
