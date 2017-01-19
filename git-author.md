# Git Author

Keep track of who is writing each page of a Gitbook with [git-author](https://plugins.gitbook.com/plugin/git-author). The plugin automatically adds the author and timestamp to each Gitbook article, including creator and last modified user by using git commits.

### Install

![git-author installation](/assets/plugins-gitauthor-install.png)

### Configure

You will have to go to book.json to add the configuration code to "pluginsConfig".

Copy the following snippet to get started:

```
"git-author":{
              "position": "bottom",
              "modifyTpl": "Last modified by {user} {timeStamp}",
              "createTpl": "Created by {user} {timeStamp}",
              "timeStampFormat": "YYYY-MM-DD HH:mm:ss"
          }
```

Now, paste the code into book.json so that it resembles the following example:

```
{
    "plugins": [
        "edit-link",
        "git-author"
    ],
    "pluginsConfig": {
        "edit-link": {
            "base": "https://github.com/archgirl/gitbook-101/tree/master",
            "label": "Edit This Page"
        },
        "git-author":{
              "position": "bottom",
              "modifyTpl": "Last modified by {user} {timeStamp}",
              "createTpl": "Created by {user} {timeStamp}",
              "timeStampFormat": "YYYY-MM-DD HH:mm:ss"
        }
    }
}
```

Now publish your Gitbook. If you get an error when publishing, copy and paste your JSON file into [JSONLint](http://jsonlint.com/) to identify any errors so they can be fixed.

### Results

_Screenshot pending_
