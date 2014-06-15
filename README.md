# Geekography :: Datasets

This repositories hosts several datasets extracted from [Github Archive](http://www.githubarchive.org/) with some additional informations such as as users gender and countries.

Data concerns approximatively 150,000 users and 250,000 repositorie, both being less than 5% of the original datasets. These sample are meant to focus on the *social coding** part of github activity, letting aside non-socialized repositories.

## Description

+ **actors_attibutes.json.gz**

Last declared attributes of users.

+ **actors_events.csv.gz**

Events count of users activity on Github.

For event types description, see [Github API documentation](https://developer.github.com/v3/activity/events/types/).

+ **actors_patterns.csv.gz**

Number of pattern occurences of users' behaviors. Each patterns represent a sequence of event types, represented by letters :

```python
        types = {
                "CommitCommentEvent": "A",
                "CreateEvent": "B",
                "DeleteEvent": "C",
                "FollowEvent": "D",
                "ForkEvent": "E",
                "GollumEvent": "F",
                "IssueCommentEvent": "G",
                "IssuesEvent": "H",
                "MemberEvent": "I",
                "PublicEvent": "J",
                "PullRequestEvent": "K",
                "PullRequestReviewCommentEvent": "L",
                "PushEvent": "M",
                "WatchEvent": "N"
        }
```

+ **repos_events.csv.gz**

Events count of repositories on Github.